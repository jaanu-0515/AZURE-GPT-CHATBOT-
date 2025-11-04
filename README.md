# 💬 Azure GPT Chatbot (Streamlit + Azure OpenAI)

An intelligent *AI chatbot* built using *Azure OpenAI* and *Streamlit*.
This project allows users to interact with a *deployed GPT model* (like gpt-4.1 or gpt-4o-mini) through a simple and elegant web interface.

## 🚀 Overview

This chatbot demonstrates the integration of *Microsoft Azure OpenAI Service* with a *Streamlit web application*.
It can be used for answering questions, brainstorming ideas, or building intelligent assistants powered by Azure’s AI models.


## ✨ Features

* 🔗 Connects to *Azure OpenAI Service* using AzureOpenAI client
* 💬 Interactive and responsive *Streamlit chat interface*
* ⚙ Customizable model deployment (supports gpt-4, gpt-4o, etc.)
* 🚀 Lightweight and easy to run locally or deploy to the cloud
* 🔒 Secure API key management using .streamlit/secrets.toml

## 🧠 Tech Stack

| Component        | Description               |
| ---------------- | ------------------------- |
| *Python*       | Core programming language |
| *Streamlit*    | Web app framework         |
| *Azure OpenAI* | GPT model integration     |
| *OpenAI SDK*   | For API communication     |


## ⚙ Setup & Installation

### 1️⃣ Clone the Repository

bash
git clone https://github.com/YOUR-USERNAME/azure-gpt-chat.git
cd azure-gpt-chat


### 2️⃣ Install Dependencies

bash
pip install -r requirements.txt


### 3️⃣ Configure Azure Settings

Open app.py and replace the placeholders with your Azure details:

python
AZURE_OPENAI_ENDPOINT = "https://<your-resource-name>.cognitiveservices.azure.com/"
AZURE_OPENAI_API_KEY = "your-azure-api-key"
AZURE_OPENAI_DEPLOYMENT = "your-deployment-name"
AZURE_OPENAI_API_VERSION = "2024-12-01-preview"


You can find these values in your *Azure AI Foundry* → Deployments → Keys & Endpoint.



## ▶ Run the App

bash
streamlit run app.py


Then open the link shown in your terminal — usually:


http://localhost:8501




## 🧾 Example Interaction

*User:*

> What is Azure AI Foundry?

*Assistant:*

> Azure AI Foundry is a unified platform by Microsoft that helps developers build, train, and deploy AI models using Azure’s cloud infrastructure and tools.



## 📂 Project Structure


📦 azure-gpt-chat
 ┣ 📜 app.py              # Main Streamlit application
 ┣ 📜 README.md           # Documentation (this file)
 ┗ 📜 requirements.txt    # Project dependencies




## 🧰 requirements.txt

Make sure your requirements.txt includes:


streamlit
openai




## 🔒 Security Notes

* Never expose your *Azure API key* in public repositories.

* Instead, store it safely in .streamlit/secrets.toml like this:

  toml
  AZURE_OPENAI_API_KEY = "your-azure-key-here"
  

* Use .gitignore to exclude sensitive files:

  
  .streamlit/
  __pycache__/
  *.pyc
  
## 🌐 Deployment Options

You can easily deploy this app to:

* *Streamlit Cloud*
* *Azure App Service*
* *Render*
* *Railway*

Each option supports Python apps with Streamlit.

Key Highlights

1.Demonstrates practical use of Azure OpenAI for building intelligent chat systems
2.Showcases integration of cloud-based AI services with modern web frameworks
3.Ideal for learning, research, or demonstrating applied AI engineering skills
4.Ready for deployment and can be extended into enterprise-grade AI assistants.

🌟 Future Enhancements

1.🗣 Add voice input and speech synthesis
2.🧠 Integrate memory for context-aware conversations
3.🌍 Deploy globally using Azure App Service
4.📊 Include chat analytics dashboard

## ⭐ Why This Project Matters

This project showcases:

* Your ability to integrate *Azure AI services* with modern web frameworks
* Your understanding of *LLM-powered app development*
* Real-world deployment skills using *Streamlit*

🏁 Conclusion

This project represents a hands-on demonstration of applied generative AI using Azure services.
It highlights how developers can bridge the gap between AI models and real-world applications with simple, powerful tools like Streamlit.
