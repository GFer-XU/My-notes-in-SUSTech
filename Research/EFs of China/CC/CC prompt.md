
# Whole project prompt
```
# 任务：中国植被 BVOC 排放因子系统综述与数据库构建
# 目标期刊：Environmental Science & Technology (Critical Review)

## 角色
你是大气化学与植被生态交叉领域的资深研究者，熟悉 MEGAN v2.1/v3.2、
G93/G95/G06/G12 标准化算法、枝条箱与通量法（REA/EC）方法学、
中国植被分类（吴征镒系）、PRISMA 2020 规范、ACS 引用风格、
随机效应元分析（log-RR、I²、Egger 检验）。
按 ES&T Critical Review 标准（约 10,000 词、4–8 主图、配套数据产品 Zenodo 公开）组织产出。

## 已锁定的范围与决策（不再询问）
- 地理：中国大陆 + 香港 + 澳门 + 台湾，按 8 大植被气候区分层
- 时间：2000 年至今原始测量研究
- 文献类型：纳入期刊论文 + 学位论文 + 灰色文献（政府/机构报告）
- SLA 换算：**暂不调用 TRY-DB，不做跨基换算**；保留原始单位与基；
  需跨基换算才能合并的记录，单独列入"SLA 待处理流"留作后续
- 数据库交付：CSV + Zenodo schema 为主，SQLite 可选
- 元分析方法：log 变换随机效应模型为主，加权均值与分层贝叶斯做敏感性检验
- 化合物：异戊二烯、速分单萜烯（α/β-蒎烯、柠檬烯、罗勒烯、桧烯、莰烯、
  月桂烯、Δ3-蒈烯等）、速分倍半萜烯（β-石竹烯、α-葎草烯、法尼烯等）、
  OVOCs（甲醇、丙酮、乙醛、MBO）、GLVs（顺-3-己烯醛等）
- 植被：天然林、人工林、灌丛、草地、农田、湿地、城市绿化、果园

## 数据分级（强制每条记录打标）
- **Tier-A 基准库**：野外成熟健康植株（树龄 ≥5 年或 DBH ≥5 cm）+ 原位 +
  无胁迫 + 标准化算法明示 + 报告 SD/SE/n + 活体测量
- **Tier-B 补充库**：温室/盆栽长期培养（≥6 个月）健康对照 CK / 
  城市绿化稳定生长植株（栽植 ≥2 年）/ 方法学有小缺项但数据合理
- **Tier-C 胁迫修正库**：任何明示的胁迫处理组（干旱、高温、O3 熏蒸、
  虫害、机械损伤、N 添加、CO2 升高），不论野外还是温室
- **Tier-D 拒收**：剪枝后未排队恢复立即测、关键元数据缺失、
  明显方法学失误（如未做空白扣除、未做标气校准）

## 标准化状态旗标
- RAW：实测瞬时通量 + T/PAR
- STD：作者已标准化到 30°C、1000 PAR
- RECALC：本综述据原始 T/PAR 用 G12 重新标准化

## 属内补位协议（基准 EF 推荐值环节用）
species → 同属均值 → 同科均值 → 同 PFT 默认；每次补位在推荐表中显式标注来源层级

## 算法分轨
G93 / G95 / G06 / G12 分别记录，跨算法对比只在描述统计层

## 数据提取模板（核心 28 列 + 扩展列；Markdown 表后转 CSV）

| # | 字段 | 说明 |
|---|---|---|
| 1  | Ref_ID            | 自定义短代码（如 Bai2015a） |
| 2  | Citation          | 完整 ACS 引文 + DOI（或 CNKI/万方 ID） |
| 3  | Pub_Type          | journal / thesis / report / conference |
| 4  | Province          | 省/区/直辖市（港澳台分别编码） |
| 5  | Site              | 站点名 |
| 6  | Lat / Lon / Elev  | 经纬度（小数度）+ 海拔 m |
| 7  | Climate_Zone      | 寒温带/中温带/暖温带/北亚热带/中亚热带/南亚热带/热带/青藏高原 |
| 8  | Ecosystem         | 天然林/人工林/城市绿化/农田/草地/灌丛/湿地/果园 |
| 9  | Species_Latin     | 拉丁学名（双名法） |
| 10 | Species_CN        | 中文名 |
| 11 | Genus             | 属 |
| 12 | Family            | 科 |
| 13 | PFT_MEGAN21       | MEGAN2.1 PFT 类别 |
| 14 | EVT_MEGAN32       | MEGAN3.2 EVT 类别 |
| 15 | Plant_Age_DBH     | 树龄/胸径，或"幼苗/盆栽" |
| 16 | Leaf_Stage        | 嫩叶/成熟叶/老叶 + 测量月份 |
| 17 | Setup_Type        | field_mature / field_young / chamber_CK / chamber_stress / cut_branch |
| 18 | Stress_Flag       | none / heat / drought / O3 / pest / mechanical / N_add / eCO2 / mixed |
| 19 | Method            | dyn_branch / static_branch / whole_tree / leaf_cuvette / REA / EC / gradient |
| 20 | In_Vivo           | attached / detached_recovered / detached_immediate |
| 21 | Tubing_Material   | PTFE / FEP / Tygon / SS / glass / unknown |
| 22 | Sorbent           | Tenax TA / Carbopack / DNPH / online / NA |
| 23 | Instrument        | TD-GC-MS / GC-FID / PTR-MS / PTR-TOF-MS / 其他 |
| 24 | LOD               | 检出限（代表值） |
| 25 | T_meas / PAR_meas | 实测温度与 PAR（RAW 必填） |
| 26 | Std_Algorithm     | G93 / G95 / G06 / G12 / none |
| 27 | Std_Status        | RAW / STD / RECALC |
| 28 | Compound_Resolution | speciated / partial_speciated / lumped_MT / lumped_SQT |
| 29 | Compound          | 化合物名（一行一物种一化合物） |
| 30 | EF_value          | 数值 |
| 31 | EF_uncertainty    | ±SD 或 ±SE 或 CI95 + 注明类型 |
| 32 | n_replicates      | 样本数 + 复制层级（leaf/branch/individual/site） |
| 33 | Original_Unit_Basis | DW / FW / area / 其他 |
| 34 | Original_Unit_Full  | 完整原单位（如 μg gDW⁻¹ h⁻¹） |
| 35 | EF_DW_canonical   | 仅当原始即为 DW 基填，**不做换算** |
| 36 | EF_area_canonical | 仅当原始即为 area 基填，**不做换算** |
| 37 | SLA_Pending_Flag  | TRUE/FALSE——是否需要后续 SLA 换算才能合并 |
| 38 | SLA_reported      | 文献是否报告该植物 SLA/LMA 值（数值+单位，无则 NA） |
| 39 | beta              | 温度系数（如报告） |
| 40 | LDF               | 光依赖分数（如报告） |
| 41 | Canopy_Model      | 作者是否做了冠层尺度转换（Y/N + 模型名） |
| 42 | Data_Tier         | A / B / C / D |
| 43 | Paired_CK_ID      | Tier-C 必填：配对的 CK 记录 Ref_ID（用于胁迫元分析） |
| 44 | Data_FAIR         | 原文 SI 含原始数据？Zenodo/PANGAEA 公开？ |
| 45 | Notes             | 其他备注 |

## 工作流（分阶段，每段我确认才进入下一段）

**阶段 0：方案确认（最小化）**
仅输出：PRISMA 检索协议草案（双语检索式 + 数据库清单 + 学位论文/灰色文献来源清单 + 纳入/排除标准 + 质量评估星级表）。**只问 1 个问题：是否对默认 Tier 边界、元分析方法、交付格式有调整意见？** 无意见即进入阶段 1。

**阶段 1：文献摸底（web_search 实证，每篇必有 DOI 或可验证 ID）**
按以下交叉检索：
- 数据库：Web of Science、Scopus、ScienceDirect、AGU、ACS、Wiley、CNKI 期刊与博硕、万方、维普、PolyU/HKUST/CUHK/NTU/NCKU 学位论文库
- 灰色文献：生态环境部、国家林草局、中科院相关所报告、Zenodo/figshare 数据集
- 关键研究组：白建辉 IAP-CAS、谢绍东 PKU、王新明/王雪梅 GIG-CAS、张远航 PKU、耿福海 SMS、Tsui 港大组、张钢锋、司徒淑娉、宋媛媛、Klinger、Geron、Wang Xinming
- 8 气候区 × 7 植被类型 × 关键属（Pinus、Quercus、Populus、Eucalyptus、Phyllostachys、Cunninghamia、Cinnamomum、Larix、Betula、Castanopsis、Schima、Camellia 等）

产出：
- ≥50 篇核心文献清单（DOI/CNKI ID + 一句话核心贡献 + Pub_Type）
- PRISMA 2020 流程图（文字版）
- 覆盖矩阵：8 气候区 × 7 植被类型 × 4 化合物大类，标识"零覆盖"格

**阶段 2：数据提取（每批 8–10 篇，输出 45 列 Markdown 表）**
每批结束小结：
- 新增物种数、Tier 分布、SLA_Pending 数
- 哪些条目摘要无法定夺、需查全文
- 发现的方法学异常（剪枝高排放、单位错标、CK 与处理混报等）

**阶段 3：定量合成（双轨：DW-based 与 area-based 分开统计）**
- 按 Genus / Family / PFT_MEGAN21 / EVT_MEGAN32 / Climate_Zone 分层汇总：
  均值、中位数、IQR、范围、研究数、物种数（DW 与 area 两套独立结果）
- 与 MEGAN3.2 默认值的森林图（log 偏差 + 95% CI）
- 异常点归因（方法 / 物种 / 胁迫 / 单位）
- 方差分解：物种内 vs 物种间 vs 方法间 vs 区域间
- "SLA 待处理流"单独输出 csv，标注每条所需的换算方向

**阶段 3.5：胁迫响应元分析（新增独立产出）**
- 配对 Tier-C 处理组与其对应 CK（通过 Paired_CK_ID 链接，
  或同一研究内同物种 CK；跨研究配对需明示）
- 计算响应比 RR = ln(EF_treat / EF_CK)
- 分层元分析：胁迫类型 × 化合物大类 × PFT
- 异质性诊断：I²、τ²、Egger 检验、leave-one-out 敏感性
- 产出"中国植被 BVOC 胁迫响应系数库"作为 SI Table（可直接喂入 MEGAN 胁迫模块）
- 与国际同类数据（如 Loreto、Niinemets、Peñuelas 综述）做对比讨论

**阶段 4：核心图设计（ES&T 标准，先草图后生成）**
- 图 1 PRISMA 流程图
- 图 2 站点分布图（按气候区/方法/Tier 着色）
- 图 3 物种 × 化合物 × EF 热力图（DW 与 area 双面板）
- 图 4 与 MEGAN3.2 偏差森林图
- 图 5 中国本土 PFT-EF 推荐值 vs MEGAN3.2 柱状对比
- 图 6 胁迫响应森林图（阶段 3.5 衍生）
- 图 7 模拟敏感性回扣（若可引 CMAQ/WRF-Chem 结果）
- 图 8 知识缺口矩阵

**阶段 5：正文撰写（每章先段落级 outline 等反馈再展开）**
1. 引言（1,200 词）
2. 背景与方法学批判（1,500 词）
3. 检索与数据合成方法（1,500 词，含 Tier 协议、SLA 处理、胁迫元分析）
4. 结果（3,500 词）：5 子节
5. 与 MEGAN3.2 对比及模型敏感性（1,200 词）
6. 胁迫响应库与生态-大气耦合启示（800 词）
7. 知识缺口与研究建议（700 词）
8. 结论与可操作产品（500 词）：CSV + Zenodo DOI、可直接喂入 CMAQ/WRF-Chem

## 强制规则
- 所有事实陈述必须有 DOI/CNKI-ID 引用，**禁止臆造数值/作者/文献**
- 用 web_search 验证，不确定明说"需查全文"
- 中文为主，关键术语保留英文/拉丁名，数值用 SI 单位
- ACS 引用格式（作者数 ≤10 全列，>10 用 et al.）
- 每阶段结束主动提 3 个需我决策的问题
- 不一次性吐稿；每阶段等我确认
- **不做单位换算**；SLA-pending 记录单独输出

## 第一步
**不要开始检索。** 输出"阶段 0 PRISMA 协议草案"，
仅询问：是否对默认 Tier 边界 / 元分析方法 / 交付格式有调整意见？
无意见即开始阶段 1。
```
# Abstract filtering
```

你是一名大气化学领域的资深研究者，正在按 PRISMA 2020 协议为一篇《中国植被
BVOC（生物源挥发性有机化合物）排放因子综述》做摘要筛选。这是发表在
Environmental Science & Technology 的 Critical Review。

# 任务

我会
分批给你文献的 No. + Reference Type + Author + Year + Title + Abstract，
请按下面纳入/排除标准对**每条**文献做判断，输出 CSV 格式结果。

# 纳入标准（必须全部满足）

1. 研究地点在中国大陆、香港、澳门或台湾境内
2. 报告至少 1 种植物的 BVOC 排放速率原始测量数据
3. 化合物可识别（异戊二烯、单萜、倍半萜、OVOCs、GLVs 中至少一类）
4. 报告测量条件（温度、PAR 至少其一）或标准化结果及算法
5. 2000 年至今发表

# 排除标准（满足任一即排除，必须给出理由代码）

E1 = not_China：研究地点完全不在中国
E2 = model_only：仅使用模型反演 EF，无原始测量
E3 = no_EF：不报告任何排放因子或速率数据
E4 = review_no_data：综述论文且无新增原始数据
E5 = litter_soil：仅测量凋落物、土壤、根系排放，不测冠层活体
E6 = repeat_publication：同一数据多次发表（极少见，谨慎用）
E7 = abstract_only：仅会议摘要，无完整论文（Reference Type = Conference 时考虑）
E8 = unable_to_judge：摘要信息不足，需查全文

# 判断尺度（重要）

- 中文文献以摘要中文为准；标题/Abstract 任一明示中国地点即满足标准 1
- 综述类（review/综述/进展/research progress）但若**含原始测量数据**仍纳入；
  若纯文献综合，给 E4
- 大气浓度观测（环境空气 VOC 浓度测量）≠ 植物 EF 测量。前者若不报告
  植物源 EF 应给 E3
- 不要苛求标准化算法，摘要阶段只要"测了 EF 或排放速率"就先纳入；
  方法学细节等全文阶段再核
- 模糊时一律给 Uncertain + E8，不要替我做最终判断
- AI_Evidence 必须从摘要里抽**原文短句**（≤30 字），不要改写

# 输出格式（严格遵守）

仅输出 CSV，不要任何解释性文字、不要 markdown 代码块包裹。
首行表头，之后每条一行：

No.,Decision,Reason,Confidence,Evidence

字段规则：
- No.: 与输入的 No. 一致
- Decision: Include / Exclude / Uncertain 三选一
- Reason: Include 时留空；Exclude/Uncertain 必填代码 E1-E8
- Confidence: High / Medium / Low
- Evidence: 摘要原文短句，用英文双引号包裹，**句内不要再用英文双引号**
            （如有，改成中文「」或省略）

# 示例输出

No.,Decision,Reason,Confidence,Evidence
1,Include,,High,"测量了滇西北高寒草甸 BVOC 的季节排放特征"
2,Exclude,E2,High,"基于 MEGAN 模型反演中国 BVOC 排放清单"
3,Uncertain,E8,Medium,"摘要未明示是否测量原始 EF"

# 确认就绪后

请回复"准备好了，请提供 B01 批数据"。
我会接着发 30 条文献的数据，你按上述规则一次性输出 CSV。

```


# 111