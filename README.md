# LawHub — 法律法规检索

面向私募基金管理人的中国法律法规检索工具，覆盖基金运作与监管、证券交易合规、反洗钱、税务、劳动人事、跨境业务等板块。

线上：https://murphymeng21.github.io/lawhub/

## 数据文件（docs/data/）

| 文件 | 内容 |
|------|------|
| `laws.json` | 法规数据（标题/发布机构/正文全文等） |

## 本地预览

```bash
cd docs && python3 -m http.server 8899
# 浏览器 http://localhost:8899
```

## 采集脚本（scripts/）

法规采集脚本（NPC 国家法律法规数据库 / CSRC / gov.cn 等数据源）：

- `download_npc.py` / `phase1_exact.py` — NPC 法规采集
- `article_search.py` — 法规检索
- `gov_rules_crawler.py` / `treaty_crawler.py` — 政府规则 / 条约采集
- `build_search_db.py` — 生成检索数据库（laws.json）

## 说明

- 原「FundLawHub」二合一网站已拆分：法规部分 = 本仓库（LawHub），案例部分 = [fundcasehub](https://github.com/MurphyMeng21/fundcasehub)。
