# AgentForge 🚀

AgentForge is an **AI content automation agent** that orchestrates multiple generative tools—LLMs, diffusion models, and motion adapters—through a unified reasoning layer.  
It can generate **captions, images, and GIFs**, remember and refine prompts, and intelligently call tools when users request improvements.  
By automating creative workflows, AgentForge reduces content creation time by **60%** and accelerates campaign launches.

---

## ✨ Features
- 📝 **Caption Generation** – Leverages LLMs to create and refine text captions.  
- 🖼 **Image Creation** – Uses diffusion models to generate high-quality images from prompts.  
- 🎞 **GIF/Animation Support** – AnimateDiff integration for prompt-based motion outputs.  
- 🛠 **Agentic Orchestration** – Main LLM decides which tool to call and generates prompts automatically.  
- 🔄 **Prompt Memory** – Stores user prompts for easy updates and iterative refinement.  
- 📡 **Platform Integration** – Ready for API-based publishing and content workflows.  

---

## 🛠 Tech Stack
- **LangChain / LangGraph** – Agent orchestration and tool management  
- **Falcon-7B** (or any LLM) – Caption generation and reasoning  
- **Stable Diffusion / DALL·E** – Image generation  
- **AnimateDiff** – GIF and motion generation  
- **React.js** – Frontend editor and user interface  
- **Hugging Face Hub** – Model hosting and checkpoint loading  

---
## 🧠 How It Works

### 🗺️ Agentic Architecture
The workflow follows a **tool-using agent design pattern**:

A[User Request] --> B[Main LLM (Agent)]

B -->|Generate prompt| C[Caption Tool (LLM)]
B -->|Generate prompt| D[Image Tool (Stable Diffusion / DALL·E)]
B -->|Generate prompt| E[GIF Tool (AnimateDiff)]
B -->|Generic query| F[LLM Direct Answer]
    
D --> G[Store/Update Prompt]
E --> G
C --> G

G --> H[User Updates]
H --> B

## 🚀 Getting Started

### Prerequisites
- Python 3.9+  
- CUDA-enabled GPU (for image/video generation)  
- Node.js (for frontend) ----- YET TO BE IMPLEMENTED :-)
