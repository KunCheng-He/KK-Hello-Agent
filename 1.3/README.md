# [1.3 动手体验：5分钟实现第一个智能体](https://datawhalechina.github.io/hello-agents/#/./chapter1/%E7%AC%AC%E4%B8%80%E7%AB%A0%20%E5%88%9D%E8%AF%86%E6%99%BA%E8%83%BD%E4%BD%93?id=_13-%e5%8a%a8%e6%89%8b%e4%bd%93%e9%aa%8c%ef%bc%9a5-%e5%88%86%e9%92%9f%e5%ae%9e%e7%8e%b0%e7%ac%ac%e4%b8%80%e4%b8%aa%e6%99%ba%e8%83%bd%e4%bd%93)

### 学习目标

- [ ] 使用 Python 从零开始构建一个智能旅行助手。
- [ ] 理解并应用智能体的核心运行机制，特别是 Thought-Action-Observation 循环。
- [ ] 感受智能体如何“思考”并与外部“工具”互动。
- [ ] 理解智能体如何进行逻辑规划以完成多步任务。

### 本节案例

本节将构建一个智能旅行助手，它会执行以下两步任务：
1.  查询北京今天的天气。
2.  根据天气情况，推荐一个合适的旅游景点。

### 导入包说明：

- `requests`：用于发送 HTTP 请求。
- `tavily-python`：用于调用 Tavily API 进行搜索。Tavily 是一个专为大型语言模型（LLM）优化的搜索引擎，旨在提供高效、真实且持久的搜索体验。该 SDK 不仅支持强大的搜索功能，还提供网页内容提取、网站遍历等高级功能，并同时支持同步和异步调用。
- `openai`：用于调用 OpenAI API 进行文本生成。