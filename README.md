# 结构生物信息学数据库导航与可视化

一份精选的结构生物信息学常用数据库参考资源，包含交互式可视化工具和数据库导航平台。

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

直接在浏览器中打开以下 HTML 文件：

```bash
# 本地开发
python -m http.server 8000  # Python 3
# 或
http-server                  # Node.js

# 访问地址
- http://localhost:8000/databases-searchable.html
- http://localhost:8000/databases-navigator.html
- http://localhost:8000/databases-timeline.html
```

### 在线访问
- [检索系统](https://github.com/PWO-CHINA/structural-bioinformatics-databases/blob/main/databases-searchable.html)
- [导航平台](https://github.com/PWO-CHINA/structural-bioinformatics-databases/blob/main/databases-navigator.html)
- [演进时间线](https://github.com/PWO-CHINA/structural-bioinformatics-databases/blob/main/databases-timeline.html)

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
- 各数据库官方文档与统计信息
- 结构生物学相关综述文献
- 清华大学学报 (自然科学版) 相关刊物

## 🛠 技术栈

- **前端框架**：React 18 + TailwindCSS
- **可视化**：原生 HTML + JavaScript
- **图标库**：Phosphor Icons
- **字体**：Inter, Noto Serif SC

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

---

**维护者**：[Qian Wenda (PWO-CHINA)](https://github.com/PWO-CHINA)  
**最后更新**：2026年2月18日