### 这是本次10th Nvidia Hackathon 的解决方案

With the development and widespread application of large language models (LLMs), we are in an era of technological innovation. In particular, retrieval-based systems are at the forefront of this technological leap. These models are not just automation tools, they are powerful assistants to improve productivity, able to interact with various tools and documents to start informed conversations.

The core topic of this Sky Hackathon is "Building Intelligent Conversation Robots Based on RAG Technology Innovation". We encourage contestants to use RAG (Retrieval-Augmented Generation) technology and combine it with NVIDIA's SDK tools to independently design and build conversational robots. Through this process, you will personally experience the complete process from data retrieval to generating dialogue, and gain an in-depth understanding of the practical application of NVIDIA SDK in the field of generative AI.


### 下面是本项目的核心模块以及对应核心实现逻辑
- data_prerprocess 模块：
    - 实现pdf/txt的读入，并用NIM api完成 text -> embedding -> faiss_index ---> save local file

- retrive module 模块：
    - 加载本地faiss -> vectorstore --> retrive --> COT/reranker --> context + chat prompt
 
- generation module 模块：
    - chat_prompt --> LLM --> self-reflect
 
- gradio
    - 设置端口/app/router       
