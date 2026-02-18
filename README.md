
# 结构生物信息学数据库导航与可视化

> ⚠️ **说明**：本项目内容由 AI (GitHub Copilot) 基于结构生物信息学领域知识自动生成并整理，目的是为研究者提供快速的数据库导航参考。**数据库链接和官方网站信息均指向真实可用的官方资源，但请以各官方网站的最新信息为准。**

---

## 📚 原文参考文献

本项目基于以下学术成果整理：

**《清华大学学报(自然科学版)》2025年第65卷第12期**
- **标题**：结构生物信息学常用数据库综述
- **作者机构**：清华大学

### 📖 原文链接（选择对应地区）

🌍 **国际版（海外访问）**：[https://oversea.cnki.net/kcms2/article/abstract?v=adNygMj_jVBuz1-yFiJY953hxNQlRJzy-S-2-nQFAb9SWU-bVP7s2BAmEAmprwg02ITt9mrMbard62Ls1P6i_ICfNtFB4o4AlDkbmD7_L4f1bkZsEBUntzNMkncj0fpvLMcsDe936kOAckGP2c0gWB-fEZWVVpzVYHbCK8WmRb4=&uniplatform=OVERSEA](https://oversea.cnki.net/kcms2/article/abstract?v=adNygMj_jVBuz1-yFiJY953hxNQlRJzy-S-2-nQFAb9SWU-bVP7s2BAmEAmprwg02ITt9mrMbard62Ls1P6i_ICfNtFB4o4AlDkbmD7_L4f1bkZsEBUntzNMkncj0fpvLMcsDe936kOAckGP2c0gWB-fEZWVVpzVYHbCK8WmRb4=&uniplatform=OVERSEA)

🇨🇳 **国内版（境内访问）**：[https://link.cnki.net/doi/10.16511/j.cnki.qhdxxb.2025.21.056](https://link.cnki.net/doi/10.16511/j.cnki.qhdxxb.2025.21.056)

> 💡 **建议**：阅读原文获取完整的数据库对比分析、性能评估和引用统计，本项目是基于原文的交互式导航补充。

---

## 📋 项目内容

本仓库包含三个核心工具：

### 1. **databases-searchable.html** - 数据库检索系统
- **描述**：支持关键词搜索、多维筛选与排序的互动式数据库查询工具
- **功能**：
  - 🔍 全文检索（数据库名称、功能、应用场景）
  - 🏷️ 按类型筛选（通用库、分类库、注释库、综合库、预测库）
  - 🏷️ 按标签筛选（结构、功能注释、疾病相关等）
  - 📊 动态排序（支持列表管理）
  - 📥 JSON 导出功能
- **适用场景**：快速查找特定功能的数据库、梳理数据库间的相互关系

### 2. **databases-navigator.html** - 数据库导航平台
- **描述**：简洁易读的数据库信息卡片展示
- **功能**：
  - 📌 分类卡片展示（通用库、分类库、注释库等）
  - 💬 核心服务与工具列表
  - 🌐 一键直达官方网站
  - 🔎 搜索与筛选功能
- **适用场景**：了解各数据库的基本信息与主要服务

### 3. **databases-timeline.html** - 数据库演进史
- **描述**：交互式时间线展示结构生物学数据库的技术演进
- **内容**：三个历史时期
  - **1950s-1990s 实验奠基**：X-ray、NMR 技术与 PDB 创立
  - **2000s-2010s 技术爆炸**：Cryo-EM、EMDB、EMPIAR 的发展
  - **2020s-Present AI 革命**：AlphaFold、深度学习与预测结构库
- **适用场景**：理解数据库体系的发展脉络与技术背景

## 🚀 快速开始

### 在线访问（GitHub Pages）
直接点击以下链接即可在浏览器中打开：

- 🏠 [**主页导航**](https://PWO-CHINA.github.io/structural-bioinformatics-databases/) — 推荐入口，包含统计概览与分类导航
- 🔍 [数据库检索系统](https://PWO-CHINA.github.io/structural-bioinformatics-databases/databases-searchable.html)
- 📚 [数据库导航平台](https://PWO-CHINA.github.io/structural-bioinformatics-databases/databases-navigator.html)  
- ⏳ [数据库演进时间线](https://PWO-CHINA.github.io/structural-bioinformatics-databases/databases-timeline.html)

### 本地开发

克隆仓库后在本地运行：

```bash
git clone https://github.com/PWO-CHINA/structural-bioinformatics-databases.git
cd structural-bioinformatics-databases

# Python 方式
python -m http.server 8000

# 或 Node.js 方式
npx http-server

# 访问地址
# http://localhost:8000/databases-searchable.html
# http://localhost:8000/databases-navigator.html
# http://localhost:8000/databases-timeline.html
```

## 📊 数据库覆盖范围

### 核心数据库

| 类型 | 代表库 | 特点 |
|------|-------|------|
| **通用库** | PDB, EMDB, EMPIAR | 原始实验结构数据、最权威 |
| **分类库** | SCOP, CATH | 结构关系分类、进化视角 |
| **注释库** | Pfam, InterPro, UniProt | 功能注释、序列分析 |
| **综合库** | UniProt | 信息中枢，跨库互联 |
| **预测库** | AlphaFoldDB, SWISS-MODEL | AI 预测、全基因组覆盖 |
| **专题库** | GPCRdb, IMGT, DisProt | 特定生物学主题深度数据 |

### 关键统计

- **PDB**：24+ 万条实验结构（截至 2025.9）
- **AlphaFoldDB**：数千万条预测结构，覆盖多物种
- **Pfam**：19,000+ 蛋白家族
- **EMDB**：3+ 万条冷冻电镜密度图

## 🔗 数据库间的互联关系

```
[实验结构] PDB/EMDB
    ↓
[结构分类] SCOP ↔ CATH
    ↓
[功能注释] Pfam → InterPro → UniProt
    ↓
[专题深入] GPCRdb, IMGT, DisProt ...
    ↓
[预测补充] AlphaFoldDB, SWISS-MODEL
```

## 💡 使用建议

### 对于结构预测研究
1. 从 **PDB** 获取实验"金标准"数据
2. 用 **SCOP/CATH** 理解结构分类
3. 参考 **AlphaFoldDB** 扩展覆盖范围
4. 用 **Pfam/InterPro** 注释功能域

### 对于药物发现
1. 检索 **PDB** 中的蛋白结构与配体复合物
2. 在 **PDBbind** 中查找亲和力数据
3. 利用 **STRING** 分析相互作用网络
4. 参考 **GPCRdb** 等专题库进行靶点设计

### 对于序列分析
1. 从 **UniProt** 开始获取规范序列
2. 使用 **Pfam** 进行结构域检索
3. 通过 **InterPro** 进行多源注释
4. 参考 **SMART** 进行信号传导域分析

## 📝 数据来源

本数据基于以下权威来源整理：
- **原文论文**：《清华大学学报(自然科学版)》2025年第65卷第12期（见上方链接）
- **数据库官方文档**：各官方网站与统计信息
- **结构生物学综述**：相关领域综述文献

### ⚡ 内容生成说明

- **工具框架**：React 18、TailwindCSS、Phosphor Icons（均使用 CDN）
- **数据整理**：AI 助手基于结构生物信息学领域知识生成
- **信息来源**：文献综述、官方文档整合
- **维护方式**：开源社区贡献制

## 🛠 技术栈

- **前端框架**：React 18 + TailwindCSS
- **可视化**：原生 HTML + JavaScript
- **图标库**：Phosphor Icons
- **字体**：Inter, Noto Serif SC
- **部署**：GitHub Pages

## 📖 进一步资源

- [wwPDB 官网](https://www.wwpdb.org/)
- [RCSB PDB](https://www.rcsb.org/)
- [EBI 数据库服务](https://www.ebi.ac.uk/)
- [AlphaFoldDB](https://alphafold.ebi.ac.uk/)

## 📄 许可

本项目仅用于教育与研究目的，各数据库遵循其原有许可证。

## 🤝 贡献

欢迎提交 Issue 或 Pull Request 以改进本项目：
- 数据库信息更新
- UI/UX 改进建议
- 新增数据库推荐
- 内容修复与完善

---

**维护者**：[Qian Wenda (PWO-CHINA)](https://github.com/PWO-CHINA)  
**AI 生成工具**：GitHub Copilot (Claude Haiku 4.5)  
**最后更新**：2026年2月18日
