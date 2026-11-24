## SIVGA-
![alt text](demo.png)
## 项目介绍 
### 是什么
本程序是基于streamlit包的python代码，是用于SIVGA耳机店人工客服测试的简要demo.
### 怎么运行 
公开网站https://yelhh5a6jhypg2qmqtg5s9.streamlit.app/，
或者把项目拉取到本地后再pip install -r requirements.txt下载所需的依赖，注意pip包要对应你的python程序。
### 工程核心亮点
1. 可切换角色的多轮对话客服，并且每个角色的对话自带记忆,切换角色时清空历史对话。u42
2. 结构化输出json格式和prompt模板化，模板可复用。u36
3. 回答范围明确，公司可上传资料，回复按资料回答。资料里没有的或者用户注入提示时拒绝回答并引导回位话术。u37
4. 错误处理不报错，程序用try except接住各种可重试和不可重试错误，st.error()是当没有配置api密钥时会在网站上显示一行错误。u28,u44
5. 密钥安全，密钥已经放在streamlit云端设置的secrets上，程序用st.secrets读取，不直接暴露在网站上。u44