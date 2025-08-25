# my-ai-agent
a simple chat ai agent that searches and gives real time updated data
# 🤖 AI Agent (n8n + OpenAI Chat Model + SERP API)

A mini no-code **AI Agent** built in **n8n** that combines:
- **OpenAI Chat Model** → natural, context-aware replies
- **SERP API** → real-time web search
- **Simple Memory** → short-term context

Unlike a static chatbot, this agent can **reason + search** to answer with up-to-date info.

---

## ✨ Features
- Agentic workflow (Model + Tools + Memory)
- Real-time lookup via SERP API
- Works inside n8n’s Chat UI
- Clean, reproducible blueprint

---

## 🧱 Architecture (Mermaid)
```mermaid
graph LR
  A[When Chat Message Received] --> B[Agent]
  B --> C[OpenAI Chat Model]
  B --> D[Simple Memory]
  B --> E[SERP API Tool]
  B --> F[Response]
