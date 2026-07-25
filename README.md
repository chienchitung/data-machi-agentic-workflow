# 《從 RAG 到 Agentic Workflow：30 天打造 Data Machi 企業知識工作流》

從 RAG、Tool Use、Agent 到 LangGraph，30 天逐步建立企業知識工作流的學習系列。

這個 repository 收錄 Data Machi 的完整 30 天文章，內容不只介紹技術名詞，也記錄如何把 AI 從「會回答問題的聊天工具」，逐步發展成能讀取企業知識、操作工具、管理工作流程，並具備可靠性與產品化思維的企業 AI 工作夥伴。

本文件站使用 [Mintlify](https://mintlify.com) 建置，網站導覽由 [`docs.json`](./docs.json) 管理。

## 系列學習路徑

整個系列分為六大篇章，每一篇包含五天內容：

| 篇章 | 天數 | 核心主題 |
| --- | --- | --- |
| 第一篇｜AI 不只要會回答，更要會工作 | Day 01–05 | 企業 AI 的定位、知識工作拆解、Prompt 與 Workflow 的差異 |
| 第二篇｜先讓 AI 找得到公司的知識 | Day 06–10 | RAG、PDF 知識庫、語意搜尋、OCR 與多模態文件 |
| 第三篇｜讓 AI 不只會讀，還會使用工具 | Day 11–15 | Tool Use、LangChain、Google Sheets、Confluence、Trello 與跨來源工作流 |
| 第四篇｜從工具呼叫進化成 Agent | Day 16–20 | Agent 決策、ReAct、Coordinator、記憶、釐清與查核 |
| 第五篇｜從黑箱 Agent 走向可控工作流 | Day 21–25 | AgentExecutor、LangGraph、平行執行、Multi-Agent 與 Human-in-the-loop |
| 第六篇｜從 Demo 走向企業級 AI 產品 | Day 26–30 | 可靠性、Agent UX、會議工作流、安全、部署與產品成熟度 |

---

## 第一篇｜AI 不只要會回答，更要會工作

從企業實際工作需求出發，釐清聊天機器人與企業 AI 工作夥伴的差異，並建立整個系列的問題意識與系統定位。

| Day | 文章 | 內容摘要 |
| --- | --- | --- |
| 01 | [企業真正需要的不是聊天機器人，而是會工作的 AI](./30-days/day-01-enterprise-ai-is-not-chatbot.mdx) | 從聊天介面出發，理解企業真正需要的是能完成知識工作的 AI。 |
| 02 | [知識工作到底包含哪些步驟？](./30-days/day-02-what-is-knowledge-work.mdx) | 把知識工作拆成 Find、Understand、Decide、Act、Track 五個階段。 |
| 03 | [為什麼 AI 知道很多，卻不一定知道公司的事情？](./30-days/day-03-why-ai-does-not-know-your-company.mdx) | 理解模型通用知識與企業私有、即時資料之間的落差。 |
| 04 | [Prompt 寫得再長，也不會自動變成工作流程](./30-days/day-04-prompt-is-not-workflow.mdx) | 區分 Prompt、Policy、Tool 與可由程式保證執行的 Workflow。 |
| 05 | [Data Machi 的誕生：從一次性分析工具到企業 AI 助理](./30-days/day-05-data-machi-origin.mdx) | 回顧 Data Machi 從資料查詢工具逐步演進成企業知識工作流的歷程。 |

## 第二篇｜先讓 AI 找得到公司的知識

進入企業 AI 的第一項核心能力：讓模型在回答前，能從 PDF、掃描文件與企業知識庫中找到真正相關且可追溯的內容。

| Day | 文章 | 內容摘要 |
| --- | --- | --- |
| 06 | [什麼是 RAG？把 AI 從閉卷考試變成開卷考試](./30-days/day-06-what-is-rag.mdx) | 用開卷考試理解 RAG 如何讓 AI 使用企業文件回答問題。 |
| 07 | [AI 如何把一本 PDF 變成可以搜尋的知識？](./30-days/day-07-pdf-to-searchable-knowledge.mdx) | 理解文件解析、Chunk 切割、Embedding、向量化與索引流程。 |
| 08 | [語意搜尋和關鍵字搜尋有什麼不同？](./30-days/day-08-semantic-vs-keyword-search.mdx) | 用實際例子比較關鍵字比對與語意相似度搜尋。 |
| 09 | [企業文件沒有想像中乾淨：掃描 PDF、表格與圖片怎麼辦？](./30-days/day-09-scanned-pdf-and-visual-content.mdx) | 理解 OCR、掃描頁、圖表、圖片與多模態文件處理。 |
| 10 | [RAG 不是萬靈丹：找得到資料，不代表完成得了工作](./30-days/day-10-rag-is-not-enough.mdx) | 釐清 RAG、Tool Use 與 Agent 的能力邊界。 |

## 第三篇｜讓 AI 不只會讀，還會使用工具

讓 AI 從查詢文件進一步接上企業系統，學會讀取結構化資料、查詢專案進度，並整合散落在不同平台中的資訊。

| Day | 文章 | 內容摘要 |
| --- | --- | --- |
| 11 | [RAG 和 Tool Use 差在哪裡？](./30-days/day-11-rag-vs-tool-use.mdx) | 區分「找回知識」與「操作外部系統」兩種不同能力。 |
| 12 | [LangChain 到底在解決什麼問題？](./30-days/day-12-what-langchain-solves.mdx) | 用非技術方式理解 LangChain 如何整合模型、Prompt、訊息與 Tool。 |
| 13 | [讓 AI 看懂 Google Sheets：Data Analyst Tool 的設計](./30-days/day-13-ai-reads-google-sheets.mdx) | 拆解自然語言如何轉成欄位辨識、資料篩選、統計與解釋。 |
| 14 | [同一個問題，答案可能散落在 Confluence 與 Trello](./30-days/day-14-confluence-and-trello.mdx) | 理解文件知識、專案狀態與結構化資料為何需要不同工具。 |
| 15 | [一個問題需要查三個系統：跨資料來源工作流怎麼設計？](./30-days/day-15-cross-source-workflow.mdx) | 用完整案例理解 Google Sheets、Confluence 與 Trello 如何合作回答企業問題。 |

## 第四篇｜從工具呼叫進化成 Agent

從單次工具呼叫進一步發展成能觀察結果、重新判斷並選擇下一步的 Agent，同時處理多輪對話、記憶與回答查核。

| Day | 文章 | 內容摘要 |
| --- | --- | --- |
| 16 | [什麼時候工具會變成 Agent？](./30-days/day-16-when-tools-become-agent.mdx) | 理解 Tool 提供能力，而 Agent 負責判斷、選擇與組合能力。 |
| 17 | [ReAct：AI 如何在思考、行動與觀察之間循環？](./30-days/day-17-react-loop.mdx) | 用 Thought、Action、Observation 理解 Agent 的基本決策循環。 |
| 18 | [Coordinator 就像專案經理：AI 如何分派任務？](./30-days/day-18-coordinator-as-project-manager.mdx) | 理解 Router、Coordinator、領域工具與上下文判斷的分工。 |
| 19 | [AI 如何記得我們剛剛談過什麼？](./30-days/day-19-agent-memory.mdx) | 區分近期對話、摘要記憶與可追溯的工具結果記憶。 |
| 20 | [不知道就問，不要亂猜：釐清、查核與零幻覺設計](./30-days/day-20-clarification-and-verification.mdx) | 理解 Clarification、Verification、Correction Protocol 與來源追溯。 |

## 第五篇｜從黑箱 Agent 走向可控工作流

當 Agent 流程愈來愈複雜，企業需要更明確的狀態、路由、權限與人工審核機制。本篇聚焦 LangGraph 與可控工作流設計。

| Day | 文章 | 內容摘要 |
| --- | --- | --- |
| 21 | [為什麼 LangChain AgentExecutor 開始不夠用了？](./30-days/day-21-why-agentexecutor-is-not-enough.mdx) | 理解黑箱 Agent loop 在企業流程、審核與控制上的限制。 |
| 22 | [LangGraph 是什麼？用 State、Node、Edge 管理 AI 工作](./30-days/day-22-what-is-langgraph.mdx) | 用流程圖與接力棒理解 LangGraph 的 State、Node、Edge。 |
| 23 | [AI 可以同時查多個系統嗎？平行工具執行的價值](./30-days/day-23-parallel-tool-execution.mdx) | 理解平行工具呼叫如何降低複合查詢的等待時間。 |
| 24 | [多個工具不等於 Multi-Agent：什麼時候才需要拆 Agent？](./30-days/day-24-tools-are-not-multi-agent.mdx) | 區分單一 Agent 多工具與真正 Multi-Agent 架構。 |
| 25 | [企業不能完全放手：Human-in-the-loop 與權限設計](./30-days/day-25-human-in-the-loop.mdx) | 理解高風險操作前的人工批准、狀態保存與權限分級。 |

## 第六篇｜從 Demo 走向企業級 AI 產品

最後五天將焦點從模型與架構轉向產品化：如何面對失敗、建立使用者信任、完成閉環工作流，並安全地部署到正式環境。

| Day | 文章 | 內容摘要 |
| --- | --- | --- |
| 26 | [模型也會塞車：Timeout、Retry 與 Fallback 怎麼設計？](./30-days/day-26-timeout-retry-fallback.mdx) | 理解企業 AI 如何面對模型逾時、限流、過載與服務不穩定。 |
| 27 | [使用者不能只看到轉圈圈：AI 工作流的 UX 設計](./30-days/day-27-agent-ux.mdx) | 理解進度提示、串流、錯誤訊息與完成狀態如何影響信任。 |
| 28 | [從會議錄音到行動項目：打造閉環知識工作流](./30-days/day-28-meeting-to-action-items.mdx) | 拆解錄音、轉錄、會議記錄、Action Items 與後續追蹤。 |
| 29 | [企業 Agent 上線前最後一哩路：安全、測試、部署與可觀測性](./30-days/day-29-security-testing-deployment.mdx) | 整理憑證、安全、測試、部署、持久化與 Debug 的產品化考量。 |
| 30 | [設計你自己的企業知識工作流 Agent](./30-days/day-30-design-your-enterprise-agent.mdx) | 用成熟度模型與設計 Canvas，完成自己的企業 AI 工作流規劃。 |

---

## 系列涵蓋的核心技術與概念

- Enterprise AI 與 Knowledge Work
- Retrieval-Augmented Generation（RAG）
- PDF Parsing、Chunking、Embedding 與 Vector Search
- OCR、Multimodal Document Processing 與 Hybrid Search
- Tool Use、LangChain 與 Structured Data Analysis
- Google Sheets、Confluence、Trello 與跨來源整合
- ReAct、Coordinator、Agent Memory 與 Verification
- LangGraph、State、Node、Edge 與 Parallel Tool Execution
- Multi-Agent、Human-in-the-loop 與權限設計
- Timeout、Retry、Fallback、Agent UX、Testing 與 Deployment

## Repository 結構

```text
.
├── 30-days/
│   ├── day-01-enterprise-ai-is-not-chatbot.mdx
│   ├── day-02-what-is-knowledge-work.mdx
│   ├── ...
│   └── day-30-design-your-enterprise-agent.mdx
├── docs.json
└── README.md
```

## 閱讀方式

建議依照 Day 01 到 Day 30 的順序閱讀。每五天形成一個完整主題，也可以依需求直接從特定篇章開始：

- 想理解企業 AI 與工作流程：從第一篇開始。
- 想建立企業文件問答系統：從第二篇開始。
- 想讓 AI 查詢不同企業系統：從第三篇開始。
- 想理解 Agent 如何自行選擇工具：從第四篇開始。
- 想導入 LangGraph 與人工審核：從第五篇開始。
- 想將 AI Demo 發展成正式產品：從第六篇開始。

## License

本系列文章內容與程式碼的使用方式，請依 repository 後續公布的 License 為準。
