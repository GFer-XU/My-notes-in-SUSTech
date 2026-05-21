
# 阶段 0：PRISMA 2020 检索协议草案

依锁定范围编制；不做检索，仅供您审阅边界与策略。

---

## 0.1 研究问题（PECO 框架）

|维度|定义|
|---|---|
|**P (Population)**|中国大陆+港澳台 8 大气候区 × 7 种植被类型中的乔木、灌木、草本、农作物|
|**E (Exposure/Condition)**|标准化测量条件（30°C / 1000 μmol m⁻² s⁻¹ PAR）或显式胁迫处理|
|**C (Comparator)**|(a) MEGAN3.2 / EVT 默认值；(b) 国际同纬度同 PFT 文献；(c) 配对 CK 组|
|**O (Outcome)**|物种级 BVOC 排放因子（异戊二烯、单萜、倍半萜、OVOCs、GLVs）+ 不确定度 + 胁迫响应比|

衍生问题：(i) 中国本土 EF 与 MEGAN3.2 默认值的系统偏差；(ii) 胁迫情境下 EF 调制系数；(iii) 知识缺口矩阵。

---

## 0.2 信息源清单

**英文数据库（5）** ==Web of Science Core Collection (SCI-E, SSCI)、Scopus、ScienceDirect、ACS Publications、Wiley Online Library、AGU (含 JGR-Atmospheres、GBC)、SpringerLink、Taylor & Francis。==

**中文数据库（4）** CNKI 中国知网（期刊+博硕论文+会议+报纸）、万方数据、维普期刊、超星读秀。

**港澳台学位论文库（6）** PolyU Electronic Theses、HKUST Repository、CUHK Theses Online、HKU Scholars Hub、台湾博硕士论文知识加值系统 (NDLTD-TW)、NCKU/NTU/NCU 机构典藏。

**预印本与数据仓库（4）** EarthArXiv、ESS Open Archive (AGU)、Zenodo、PANGAEA、figshare、NSF EDI、ORNL DAAC。

**政府与机构灰色文献（6）** 生态环境部环境规划院、国家林业和草原局调查规划设计院、中科院大气物理所/地球化学所/华南植物园/植物所/沈阳应用生态所/西双版纳植物园技术报告、CARB/EPA/EEA 跨国比对报告（仅作对照）、IGAC/MOZAIC 项目报告、香港环保署 EPD 报告。

**会议论文集** AGU Fall Meeting、EGU、AAAR、ACCESS、中国气象学会、中国环境科学学会年会摘要集。

---

## 0.3 双语检索式

### 英文（WoS/Scopus/ScienceDirect 范式，TS = topic）

```
TS=(
  ("biogenic volatile organic compound*" OR BVOC OR "biogenic VOC*" OR
   isoprene OR monoterpene* OR sesquiterpene* OR
   "α-pinene" OR "alpha-pinene" OR "β-pinene" OR "beta-pinene" OR
   limonene OR ocimene OR sabinene OR myrcene OR camphene OR
   "Δ3-carene" OR "delta-3-carene" OR caryophyllene OR humulene OR
   farnesene OR methanol OR acetone OR acetaldehyde OR MBO OR
   "2-methyl-3-buten-2-ol" OR "green leaf volatile*" OR GLV OR
   "cis-3-hexenal" OR "hexenyl acetate")
  AND
  ("emission factor*" OR "emission rate*" OR "emission capacit*" OR
   "emission potential" OR "standard emission" OR "basal emission" OR
   flux OR exchange OR "emission strength")
  AND
  (China OR Chinese OR PRC OR Tibet OR Tibetan OR Xizang OR
   Taiwan OR Taiwanese OR "Hong Kong" OR Macau OR Macao OR
   Yunnan OR Sichuan OR Guangdong OR Guangxi OR Hainan OR
   Fujian OR Zhejiang OR Jiangsu OR Jiangxi OR Hunan OR Hubei OR
   Anhui OR Shandong OR Henan OR Hebei OR Shanxi OR Shaanxi OR
   Gansu OR Qinghai OR Ningxia OR Xinjiang OR "Inner Mongolia" OR
   Heilongjiang OR Jilin OR Liaoning OR Beijing OR Shanghai OR
   Tianjin OR Chongqing OR Guizhou)
)

时间窗：2000-01-01 至检索日
文献类型：Article OR Review OR Proceedings Paper OR Data Paper
语种：English
```

```

```
### 中文（CNKI/万方 范式）

```
(主题 = "生物源挥发性有机物" OR "生物挥发性有机物" OR BVOC OR
         "生物排放" OR 异戊二烯 OR 单萜 OR 单萜烯 OR 倍半萜 OR
         蒎烯 OR α-蒎烯 OR β-蒎烯 OR 柠檬烯 OR 罗勒烯 OR 桧烯 OR
         月桂烯 OR 莰烯 OR 蒈烯 OR 石竹烯 OR 葎草烯 OR 法尼烯 OR
         甲醇 OR 丙酮 OR 乙醛 OR MBO OR "绿叶挥发物")
AND
(主题 = 排放因子 OR 排放速率 OR 排放通量 OR 标准排放 OR
         基础排放 OR 释放速率 OR 排放潜力 OR 通量)
AND
(主题 = 植被 OR 森林 OR 灌丛 OR 草地 OR 农田 OR 果园 OR 城市绿地 OR
         乔木 OR 灌木 OR 林木 OR 树种 OR 阔叶林 OR 针叶林 OR
         常绿 OR 落叶 OR 竹 OR 油松 OR 马尾松 OR 樟 OR 桉)
学科限定：环境科学、大气科学、生态学、林学、植物学
时间：2000–至今
文献类型：期刊 + 博硕士 + 会议 + 报纸（剔重）
```

### 灰色文献定向检索

对 6 个机构网站做站内 site: 检索（用 Google Scholar 与机构原生站内搜索双轨）： `site:nies.org / site:cern.ac.cn / site:gov.cn "BVOC" OR "生物源" filetype:pdf`

---

## 0.4 纳入/排除标准

### 纳入（必须全部满足）

1. 报告至少 1 种中国境内（含港澳台）野外或受控条件下的活体植物 BVOC 排放速率
2. 化合物可识别（speciated 或 lumped_MT / lumped_SQT 明示）
3. 报告测量条件（T、PAR 至少其一）**或** 标准化结果及算法
4. 报告样本量与重复方式
5. 2000 年至今发表
6. 中英文全文可获取（含通过馆际互借）

### 排除

1. 模型反演 EF 而无原始测量
2. 凋落物、土壤、根系排放（本综述聚焦冠层活体）
3. 仅作 CMAQ/WRF-Chem 输入清单二次引用，无原始测量
4. 重复发表（同数据多刊）——保留信息最全版本
5. 关键元数据缺失且通讯作者无回应（计入 Tier-D 并记录）
6. 综述/会议摘要无原始数据（用于背景讨论而不入库）

### 全文复核触发条件

- 摘要数值与正文常识量级偏差 >10×
- 摘要未明示单位基（DW/FW/area）
- 摘要未明示标准化状态
- 涉及罕见或新记录物种

---

## 0.5 数据提取与质控流程

```
摘要筛选（双人独立，Cohen κ ≥0.8 进全文）
        ↓
全文复核（双人独立 → 分歧仲裁）
        ↓
45 列模板录入（每条强制 Tier 与 Std_Status 旗标）
        ↓
随机 10% 二次核对（≤2% 错误率为通过）
        ↓
入"主库 / SLA 待处理流 / 胁迫库"三流
        ↓
描述统计 + 元分析
```

---

## 0.6 质量评估星级表（★ 1–5，对应 Tier A–D 校验）

|维度|1★ 条件|备注|
|---|---|---|
|**代表性**|野外成熟健康植株（DBH≥5 cm 或 树龄≥5 a）；或长期培养（≥6 mo）健康 CK|幼苗/盆栽短养无 ★|
|**方法学**|闭式动态枝箱 + PTFE/FEP 管路 + 标气校准 + 空白扣除四项全|缺一项扣 0.5★|
|**化学分辨**|TD-GC-MS 或 PTR-TOF-MS 物种级；GC-FID 集总 −0.5★|仅 lumped 给 0.5★|
|**不确定度**|报告 SD/SE/CI 与 n、复制层级|仅给均值 0★|
|**标准化**|明示 G06/G12 标准化或提供 T/PAR 可重算|二者皆缺 0★|

**对照 Tier**：≥4.5★ → Tier-A；3.0–4.0★ → Tier-B；任何胁迫标识 → 进 Tier-C（不参与 Tier-A 池）；<3.0★ 且无胁迫标识 → Tier-D。

**双评一致性**：κ ≥0.8 直接接受；0.6–0.8 仲裁；<0.6 重新培训评分员。

---

## 0.7 偏倚与异质性诊断方案

|检验|用途|
|---|---|
|Egger / Begg|发表偏倚|
|Funnel plot 视觉判读|小样本研究偏倚|
|I² + τ² + Q|异质性量化（>75% 视为高异质）|
|Leave-one-out|单研究敏感性|
|Cumulative meta|时间累积稳健性|
|Subgroup (PFT/Zone/Method)|异质源解释|

---

## 0.8 PRISMA 流程图占位（待阶段 1 实测填数）

```
鉴定（Identification）
├─ 英文库 N=___
├─ 中文库 N=___
├─ 学位论文 N=___
└─ 灰色文献 N=___
       │ 去重 −___
       ▼
筛选（Screening）摘要 N=___
       │ 排除 −___ （理由分类计数）
       ▼
合格（Eligibility）全文 N=___
       │ 排除 −___ （Tier-D / 数据缺失 / 重复发表）
       ▼
纳入（Included） N=___
   ├─ Tier-A: ___
   ├─ Tier-B: ___
   └─ Tier-C: ___
```

---

## 0.9 预登记与可重复性

- 协议拟在 OSF 预登记（最终稿件投稿前公开）
- 检索语句、筛选记录、提取表、分析脚本（R / Python）全程进 Zenodo
- Zenodo schema 草案：`csvw-metadata.json` + `datapackage.json` 双轨
- 代码许可：MIT；数据许可：CC-BY 4.0

---


下面按 **WoS 检索 → 导入 EndNote → 双库去重 → PRISMA 筛选 → PDF 获取 → 分类标签** 顺序展开，全部按科研规范写。

---

# 1. WoS 检索的科研规范

## 1.1 检索前必做的"预登记"动作

打开 WoS 之前，先在电脑上建一个文件夹 `BVOC_review/01_search_log/`，里面预先建好这张表（Excel 或 Markdown 都行）：

| 字段           | 说明                                       |
| ------------ | ---------------------------------------- |
| Search_ID    | S001、S002…按时间编号                          |
| Database     | WoS Core Collection / Scopus / CNKI / 万方 |
| Query_string | **原文逐字粘贴**，包括所有括号                        |
| Date_run     | 检索执行日期                                   |
| Time_window  | 2000-01-01 to 2026-05-21                 |
| Filters      | 文献类型、语言                                  |
| N_hits       | 返回篇数                                     |
| Export_file  | 导出文件名（如 `S001_WoS_2026-05-21.ris`）       |
| Notes        | 例外情况                                     |

**这张表是综述能发表的硬要求**。审稿人和 PRISMA 2020 都要求你能在论文里说"2026-05-21 检索 WoS Core Collection，返回 N 篇"，并能让别人按你的查询语句复现这个数字。**不记录 = 不可复现 = 退稿风险**。

## 1.2 WoS Core Collection 实际操作

WoS 网页（webofscience.com）→ 顶部切换到 **Web of Science Core Collection**（不是 All Databases，All Databases 检索方式不规范）。

**步骤 A：粘贴检索式**

进入 Advanced Search 而不是 Basic Search。在 Basic Search 框里写复杂布尔会被截断，Advanced Search 才支持长字符串。

把阶段 0 给你的英文检索式直接粘进 Advanced Search 框。**不要改任何字符**，包括 `TS=`、括号、`AND/OR/NOT`。

**步骤 B：精炼**

返回后用左侧 Refine results 面板：

- Document Types: 勾 Article、Review Article、Proceedings Paper、Data Paper
- Languages: 勾 English
- Publication Years: 2000-2026

**不要在这一步勾"WoS 分区""高被引"等过滤器**——后期筛选要看的是研究质量与契合度，不是 IF。

**步骤 C：记录命中数**

无论结果是 50 还是 5000 篇，记下 N_hits。然后立即填进 search_log 表，截图存档到 `01_search_log/screenshots/S001_WoS.png`。

## 1.3 数百篇怎么办？正确顺序是"先全部导出，再筛选"

**不要在 WoS 网页上逐篇看摘要筛选**。这是新手最常犯的错误，因为：

- 网页操作不留痕迹
- 漏选漏看无法回溯
- 中间换电脑就丢了

正确做法是**全部导出到 EndNote**，所有筛选动作都在 EndNote 里做（或专门的 Rayyan 网页工具），带 audit trail。

**WoS 导出操作**：

1. 全选所有结果（页面右上 "Select All on Page" → 出现提示 "Select N records" → 点 "Add to Marked List"）
2. 重复换页，直到所有结果都加进 Marked List
3. 进 Marked List → Export → EndNote → 选 "Full Record" → 下载得到 `savedrecs.ris` 文件
4. 改名为 `S001_WoS_2026-05-21.ris` 存进 `01_search_log/exports/`

**WoS 单次最多导出 1000 篇**。如果 N_hits > 1000，分批导：1-1000、1001-2000……，文件名加后缀 `_part1.ris`、`_part2.ris`。

---

# 2. EndNote 库的科研规范配置

## 2.1 建一个库不是多个库

新手最常踩的坑：每个数据库建一个 EndNote 库。**错的**。

正确做法：**只建一个主库** `BVOC_China_review.enl`，所有数据库结果都导进这一个库。原因：

- 跨库去重必须在同一个库内做
- EndNote 的 Groups（分组）功能可以模拟"子库"，但物理上是一个库
- 备份只备一个文件

操作：EndNote → File → New → 命名 `BVOC_China_review.enl` → 选保存位置（**放进 Dropbox/OneDrive 同步盘，不要放桌面**）。

## 2.2 必须建的 Group 结构

在 EndNote 里建以下分组（Groups 面板右键 → Create Group / Create Group Set）：

```
📁 1_Sources（来源分组集，标记来自哪个数据库）
   ├─ WoS_raw
   ├─ Scopus_raw
   ├─ ScienceDirect_raw
   ├─ CNKI_raw
   ├─ Wanfang_raw
   ├─ Theses_raw
   └─ GreyLit_raw

📁 2_Screening（筛选阶段标记）
   ├─ Stage1_duplicates_removed
   ├─ Stage2_abstract_screened
   ├─ Stage2_excluded（按理由再分子组：not_China / model_only / no_data / etc）
   ├─ Stage3_fulltext_needed
   ├─ Stage3_included
   └─ Stage3_excluded

📁 3_Final_database（最终入库）
   ├─ Tier_A
   ├─ Tier_B
   ├─ Tier_C_stress
   └─ Tier_D_rejected_kept_for_record
```

**Group Set 是文件夹，Group 是文件**。每条文献可以同时属于多个 Group，所以一篇文献可以同时在 `WoS_raw` 和 `Stage2_abstract_screened` 里——这正是我们要的。

## 2.3 WoS 导入 EndNote

EndNote 里：File → Import → File → 选 `S001_WoS_2026-05-21.ris` → Import Option 选 "Reference Manager (RIS)" → Duplicates 选 "Import All"（先全部导，去重后面统一做）→ 点 Import。

导入后 EndNote 左侧 "Imported References" 会显示这次新增的条数。**立即**把这批条目拖进 `WoS_raw` 分组：Ctrl+A 全选 → 拖到 `WoS_raw` Group 上。

记下：S001 导入了 X 篇，与 N_hits 应该相等，如不等就是导入出错（常见原因：RIS 文件分批未合并）。

## 2.4 跨库去重

把所有数据库都导入主库之后，做一次去重。

EndNote → References → Find Duplicates → 弹出比对窗口 → 逐对人工确认 → 选 Keep This Record。

**关键设置**：Edit → Preferences → Duplicates → 勾选比对字段为 Author + Year + Title + Volume + Issue。不要只比 DOI（同一篇文章不同数据库可能 DOI 字段缺失）。

去重后所有保留下来的文献拖进 `Stage1_duplicates_removed` Group。**记录**：去重前 X 篇，去重后 Y 篇，删了 X-Y 篇。这个数字直接进 PRISMA 流程图。

---

# 3. 摘要筛选阶段的科研规范

数百篇全文不可能都读，但摘要必须每篇看一遍。这是 PRISMA 的硬要求。

## 3.1 工具选择：EndNote 还是 Rayyan

**EndNote** 优点：本地、不依赖网络、能做引文管理。缺点：没有为系统综述设计的筛选界面，标记筛选状态要靠 Custom Fields 或 Groups 凑。

**Rayyan**（rayyan.ai，免费）：专门为系统综述设计。优点：界面就是为"看摘要 → 决定 include/exclude → 标排除理由"设计的，支持盲筛、双人独立筛、记录 κ 一致性。缺点：要上传到云端（PRISMA 综述这是行业标准做法，不算问题）。

**强烈建议**：摘要筛选用 Rayyan，文献管理与正文写作用 EndNote。两个工具并用是国际综述论文的标准做法。

## 3.2 Rayyan 操作流程

1. 注册 rayyan.ai
    
2. New Review → 命名 BVOC_China_review
    
3. Add references → 上传 EndNote 导出的 RIS 文件（EndNote 里 File → Export → 格式选 RIS）
    
4. Rayyan 自动再做一次去重（与 EndNote 的去重独立做，两次去重叠加更稳）
    
5. 进入筛选界面，每篇摘要前有 Include / Maybe / Exclude 三个按钮
    
6. **建立 Exclusion Reasons 标签**：进入 Settings 加预设理由：
    
    - `not_China`（非中国境内）
    - `model_only`（仅模型反演无测量）
    - `no_EF`（不报告排放因子）
    - `review_no_data`（综述无原始数据）
    - `litter_soil`（凋落物/土壤排放）
    - `repeat_publication`（重复发表）
    - `abstract_only`（仅会议摘要）
    - `unable_to_judge`（摘要信息不足，需全文）
7. 逐篇点 Include / Exclude，Exclude 必须选一个理由
    
8. 不确定的点 Maybe，后面集中处理
    
9. 全部过完一遍后，导出 Excluded 列表与 Included 列表（CSV 格式）
    

## 3.3 双人筛选与一致性

ES&T Critical Review 级别的综述**强烈建议**双人独立筛选。如果只有您一个人：

- 自己筛完一遍后，**间隔 1 周再筛一遍**（同样的人,不同的时间点），比对两次结果
- 不一致的条目重看摘要做最终决定
- 记下两次一致率（不算 κ 但能展示自我核查严谨性）

如果有合作者/学生：

- 两人独立筛同一批摘要
- 用 Rayyan 的 Blind mode（互相看不到对方决定）
- 全部筛完解盲，计算 Cohen's κ（Rayyan 自动算）
- κ ≥ 0.8 接受、0.6-0.8 仲裁、<0.6 重新培训

## 3.4 摘要筛选的判断尺度

每篇摘要看以下几点（按顺序，遇排除直接 Exclude，不必继续看下面的）：

1. **地理**：研究地点在中国大陆+港澳台吗？不是 → `not_China`
2. **数据类型**：有原始 EF 测量吗？只是模型反演 → `model_only`
3. **完整性**：摘要里至少能看出测了某物种、某化合物吗？只笼统说"测了 BVOC" → `unable_to_judge`（看全文）
4. **生态系统**：测的是活植物吗？凋落物/土壤/微生物 → `litter_soil`
5. **重复**：作者+年份+物种+地点高度相似已有条目 → `repeat_publication`
6. 全部通过 → Include

**摘要筛选不要苛求标准化算法、不要苛求单位基**。这些只有全文才能判断，摘要阶段先把明显不符合的剔掉就行。

## 3.5 筛选记录与回填 EndNote

Rayyan 筛完后导出 Included CSV，回到 EndNote：

- 把 Included 文献对应的条目拖进 `Stage2_abstract_screened` Group
- Excluded 的拖进 `Stage2_excluded` 下对应理由的子组
- 这样 EndNote 里永远能查到"为什么这篇被排除"

---

# 4. PDF 获取的科研规范

通过摘要筛选的文献（预计 ~130 篇）需要拿全文。

## 4.1 获取顺序（从易到难）

1. **机构订阅**（绝大多数 Elsevier/Wiley/ACS/Springer 文章走这条路）
    - 在校园网内或开 VPN 访问机构图书馆数据库
    - 进数据库后从 DOI 直接打开，自动认证
2. **作者主页 / ResearchGate**：很多作者会上传 postprint
3. **预印本平台**：EarthArXiv、ESS Open Archive、bioRxiv 上常有同篇预印版
4. **馆际互借**（ILL）：机构图书馆都提供，3-7 天到货
5. **直接邮件向通讯作者要**：邮件简短说明"在做综述、希望读您 20XX 的论文 X、附 DOI"，回复率比想象中高（>50%）
6. **学位论文**：CNKI / 万方 / ProQuest / 港澳台 NDLTD-TW

**不要用 Sci-Hub 等盗版站**。综述发表时审稿人不会问，但你写"Data availability"声明时心里要踏实。

## 4.2 PDF 文件命名与存放

建立目录结构：

```
BVOC_review/
├── 01_search_log/
├── 02_endnote/
│   └── BVOC_China_review.enl
├── 03_rayyan_exports/
├── 04_pdfs/
│   ├── Klinger2002_JGR.pdf
│   ├── Wang2003_AtmosEnviron.pdf
│   ├── Bai2006_AtmosEnviron.pdf
│   └── ...
├── 05_extraction/（阶段 2 用）
└── 06_analysis/（阶段 3 用）
```

**PDF 文件命名严格遵守**：`FirstAuthorLastnameYYYY_JournalShortname.pdf`。不要用空格、中文、特殊字符。

**自动化**：EndNote 有个功能 References → Find Full Text，配合机构订阅能自动下载一部分 PDF 并挂到对应条目上。挂上后 EndNote 条目左侧会显示纸夹图标。

但这个功能成功率约 40-60%，剩下的还是要手动。手动下载的 PDF 保存到 `04_pdfs/` 后，回到 EndNote 对应条目 → 右键 → File Attachments → Attach File → 选 PDF。这样在 EndNote 里点条目就能直接打开 PDF。

## 4.3 拿不到全文的处理

有些早期中文期刊、灰色文献、会议论文实在拿不到。这些条目移到 `Stage3_excluded` 下新建子组 `unavailable_fulltext`，**保留在数据库里作为已知存在但无法获取的记录**。

写综述时在 Limitations 节会提到："N 篇文献因全文不可获得未纳入定量合成"。这是诚实做法。

---

# 5. PDF 拿到后的进一步分类

## 5.1 全文复核标记

得到 PDF 后做一遍全文复核（这是 PRISMA 的 Eligibility 阶段）。每篇 PDF 看以下要素，记在一张筛选表里：

|Ref_ID|中国境内?|活体植物?|报告 EF?|报告 T/PAR 或标准化?|报告 n 与不确定度?|决定|
|---|---|---|---|---|---|---|
|Klinger2002|Y|Y|Y|Y(G93)|Y|Include|
|...|||||||

筛选表存为 `BVOC_review/03_rayyan_exports/fulltext_screening.xlsx`。

通过的文献拖进 EndNote `Stage3_included`。

## 5.2 主题分类标签（在 EndNote 里加 Keywords 或 Custom Fields）

PDF 拿到、入库之后，每篇加几个分类标签便于阶段 2 提取时按主题取用：

- **Climate_Zone**: cold_temperate / mid_temperate / warm_temperate / N_subtropical / mid_subtropical / S_subtropical / tropical / TP
- **Ecosystem**: natural_forest / plantation / urban / shrubland / grassland / cropland / wetland / orchard
- **Method**: dynamic_branch / static_branch / leaf_cuvette / REA / EC / gradient / whole_tree
- **Compounds**: ISO_only / ISO_MT / ISO_MT_SQT / OVOC_inclusive / GLV_inclusive
- **Stress**: none / drought / heat / O3 / N / multi

EndNote 用 Custom 1-8 字段存这些（Tools → Define Custom Fields）。或者更省事用 Keywords 字段，分号隔开。

阶段 2 提取时按这些标签筛选，比如取所有 `Method=dynamic_branch AND Compounds=ISO_MT_SQT` 的文献，正好是高质量近 5 年组。

---

# 6. 全流程时间预估

|阶段|工作内容|估时|
|---|---|---|
|数据库检索 + 导出|跑 5 个英文库 + 4 个中文库各 1 次|4-6 小时|
|EndNote 导入 + 去重|全部导入 + Find Duplicates 人工确认|2-3 小时|
|Rayyan 摘要筛选|假设去重后 500 篇，每篇 1 分钟|8-10 小时（可分多天）|
|PDF 获取|130 篇，平均每篇 5-10 分钟|10-20 小时（可挂着做别的）|
|全文复核|130 篇，每篇 15-30 分钟|30-65 小时|
|入库标签|通过复核约 90 篇|3-5 小时|

**总计 60-110 小时**。这是文献综述里必经的最枯燥但必须的阶段。完成它之后阶段 2 提取才有意义。

---

# 7. 三个建议先决策

**E1 — Rayyan 是否使用**：注册 rayyan.ai 免费用，还是只用 EndNote 完成所有筛选？我建议用 Rayyan，但您可能有机构习惯。

**E2 — 双人筛选**：是您一人做还是有合作者？这关系到下一步我要不要给您"自我盲筛 + 间隔 1 周"的具体操作模板。

**E3 — 中文库检索**：CNKI / 万方的检索界面与 WoS 差很多，导出 RIS 也有坑（如作者名拼音问题）。要不要我下一步专门写"CNKI/万方检索 + 导入 EndNote 的避坑指南"？这是真正容易出问题的地方。

回答 E1-E3 之后，我下一步给您具体操作模板（如 CNKI 导出步骤、EndNote 自定义字段设置截图说明、Rayyan 双人盲筛配置）。