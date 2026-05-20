
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

**英文数据库（5）** Web of Science Core Collection (SCI-E, SSCI)、Scopus、ScienceDirect、ACS Publications、Wiley Online Library、AGU (含 JGR-Atmospheres、GBC)、SpringerLink、Taylor & Francis。

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
NOT TS=("anthropogenic" AND NOT "biogenic")
时间窗：2000-01-01 至检索日
文献类型：Article OR Review OR Proceedings Paper OR Data Paper
语种：English
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

## ⚠ 唯一待决策问题

**对默认 Tier 边界、元分析方法（log-RR 随机效应为主 + 加权均值 + 分层贝叶斯做敏感性）、交付格式（CSV + Zenodo schema 为主，SQLite 可选）三项，是否有调整意见？**

无意见请回复"进入阶段 1"，将启动 web_search 实证检索并交付 ≥50 篇核心文献清单 + 覆盖矩阵。