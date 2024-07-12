### 这是本次10th Nvidia Hackathon 的解决方案

- data_prerprocess 模块：
    - 实现pdf/txt的读入，并用NIM api完成 text -> embedding -> faiss_index ---> save local file

- retrive module 模块：
    - 加载本地faiss -> vectorstore --> retrive --> COT/reranker --> context + chat prompt
 
- generation module 模块：
    - chat_prompt --> LLM --> self-reflect
 
- gradio
    - 设置端口/app/router       
