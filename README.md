# chainlit-langchain-chatbot

Chainlit 是一个开源 Python 包，可以以惊人的速度构建和共享 LLM 应用程序，彻底改变了我们构建和共享语言模型应用程序的方式。将 Chainlit API 集成到您现有的代码中，在几分钟内生成类似 ChatGPT 的界面！

Chainlit 与 Streamlit 的不同之处在于它能够可视化模型的中间步骤和思维过程，让您深入了解它如何获得特定的生成输出。这使其成为理解和调试语言模型决策处理的强大工具。
在本文中，我们将展示如何在本地安装 Chainlit，重点介绍其主要功能，并探索其与不同应用程序的无缝集成。了解 Chainlit 在 UI 和交互方面的优势。

# 快速开发

1）、将代码下载到本地。
```shell
git clone https://github.com/Crossme0809/chainlit-langchain-chatbot.git
cd chainlit-langchain-chatbot
```
2）、将 example.env 重命名为 .env，并使用 cp example.env .env 并输入 OpenAI API 密钥，如下所示。从此 URL 获取 OpenAI API 密钥。如果您还没有的话，您需要在 OpenAI 网站中创建一个帐户。
```properties
OPENAI_API_KEY=your_openai_api_key
```
3）、创建一个 virtualenv 并激活它
```shell
python3 -m venv .venv && source .venv/bin/activate
```
4）、如果你有 python 3.11，那么上面的命令就可以了。但是，如果你的 python 版本低于 3.11。使用 conda 更容易。首先确保你已经安装了 conda。然后运行以下命令。
```shell
conda create -n .venv python=3.11 -y && source activate .venv
```
5）、在终端中运行以下命令来安装必要的 python 包：
```shell
pip install -r requirements.txt
```
5）、在终端中运行以下命令来启动聊天 UI：
```shell
chainlit run pdf_qa.py -w
chainlit run txt_qa.py -w
chainlit run pdf_txt_qa.py -w
chainlit run csv_qa.py -w
```

您的浏览器将自动显示一个显示您的聊天机器人的新选项卡，您也可以通过默认地址 localhost:8000 手动打开它。
