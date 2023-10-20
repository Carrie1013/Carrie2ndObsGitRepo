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

- 任务相关task-specific指令prompt优化LLM

### CoT - Chain of Thought
- 3 of the most common methods for improving the performance of any LLM:
	- Prompt Engineering
	- Retrieval Augmented Generation (RAG)
	- Parameter Efficient Fine-Tuning (PEFT)
- Thought-based Prompt Engineering![[Pasted image 20231019104432.png]]

'LLM stands for Master of Laws. It is a postgraduate degree in law that typically focuses on a specific area of legal study. It is designed for students who have already completed a Juris Doctor (JD) or equivalent law degree and wish to further specialize or gain advanced knowledge in a particular field of law. The program usually involves coursework, research, and sometimes a thesis or dissertation.',

'LLM stands for Master of Laws. It is a postgraduate degree in law that allows students to specialize in a specific area of legal study. The program typically involves in-depth coursework and research, and provides advanced knowledge and skills in the field of law.',

'LLM stands for Master of Laws, which is a postgraduate degree in law that is internationally recognized. It is typically pursued by individuals who have already completed a law degree and wish to specialize in a specific area of law or enhance their legal knowledge and skills. The LLM degree program focuses on advanced legal analysis, research, and understanding of the law.',

"LLM stands for Master of Laws, which is a postgraduate degree in law. It is a specialized program that allows students to gain advanced knowledge and skills in a specific area of law. The degree typically requires a bachelor's degree in law or a related field, and emphasizes research, critical analysis, and legal writing.",

'LLM stands for Master of Laws and is an advanced law degree that focuses on a specific area of legal expertise. It is typically pursued by individuals who already hold a law degree and want to specialize in a particular field of law or pursue a career in academia or research. The degree is offered by many universities and usually requires one year of full-time study.'


​