https://platform.openai.com/account/usage
### LangChain
- 模块
	- models
		- language models：语言模型
			- 1. LLMs：封装了接受文本输入并返回文本输出的 API；
			- 2. Chat Models：封装了接受聊天消息输入并返回聊天消息输出的模型。
			- 存在细微差别，但使用它们的接口是相同的。可以导入这两个类，实例化它们，然后在这两个类上使用 predict 函数并观察它们之间的区别。
		- text embedding models：文本嵌入模型
			- (eg.) model name = 'text-embedding-ada-002'
			  tokenizer = 'cl100k_base'
			  max input tokens = 8191
			  output dimensions = 1536
	- prompts
		- LangChain提供了Prompt Template类来构建使用多个值的prompt。提示的重要概念包括提示模板、输出解析器、示例选择器和聊天提示模板。
	- indexes
	- memory
	- chains
	- agents
- LangChain核心模块
- Agent执行逻辑