# 🧠 SnareDrop AI Hub

Welcome to **SnareDrop AI Hub** — your all-in-one, self-hosted AI stack powered by open models and terminal sorcery. This system gives you a local-first, Warp-like terminal AI assistant, real-time chat interfaces, flow-based automation tools, and full Ollama-backed LLM power — all running on your VPS.

> 🔐 100% Private | ⚡️ Local Models | 🧩 Modular | ☠️ Warp-on-steroids for Linux nerds

![Status](https://img.shields.io/badge/status-live-green?style=for-the-badge&logo=vercel)
![License](https://img.shields.io/badge/license-Cyberpunk%20Copyleft-9c27b0?style=for-the-badge)
![Built%20for](https://img.shields.io/badge/built%20for-twist3dkinkst3r.com-ff1493?style=for-the-badge&logo=cloudflare)

![Ollama](https://img.shields.io/badge/Ollama-local--LLMs-4caf50?style=flat-square&logo=linux)
![OpenInterpreter](https://img.shields.io/badge/Interpreter-AI%20Shell-blueviolet?style=flat-square&logo=gnome-terminal)
![Flowise](https://img.shields.io/badge/Flowise-LLM%20Workflow-03a9f4?style=flat-square&logo=airflow)
![OpenWebUI](https://img.shields.io/badge/OpenWebUI-Chat%20Interface-e91e63?style=flat-square&logo=webcomponents)

![Docker](https://img.shields.io/badge/Dockerized-yes-2496ed?style=flat-square&logo=docker)
![Coolify](https://img.shields.io/badge/Coolify%20Ready-yes-ff5722?style=flat-square&logo=githubactions)
![Dokploy](https://img.shields.io/badge/Dokploy%20Compatible-yes-795548?style=flat-square&logo=nginx)




---

## 📦 What's Inside

| Service           | Description                                                   | Port   |
|------------------|---------------------------------------------------------------|--------|
| 🧠 Ollama         | Local LLM model server (LLaMA3, Code Llama, Mistral, etc.)    | 11434  |
| 🔮 Open Interpreter | AI assistant that runs + explains terminal commands           | CLI    |
| 💬 OpenWebUI      | ChatGPT-style web UI for local LLMs (Ollama, LocalAI, etc.)   | 3002   |
| 🧠 Flowise         | Drag-and-drop LLM app builder (LangChain-style workflows)     | 3003   |

---

## 🚀 Quick Start

1. Clone the repo:

```bash
git clone https://github.com/YOUR_USERNAME/snaredrop-ai-hub.git
cd snaredrop-ai-hub
````

2. Create your `.env` file:

```bash
cp .env.example .env
# (edit it as needed)
```

3. Launch the stack:

```bash
docker compose up -d
```

4. Pull a model (e.g. LLaMA3):

```bash
docker exec -it ollama ollama run llama3
```

5. Run Open Interpreter:

```bash
docker exec -it interpreter interpreter
```

---

## 🌐 Web Interfaces

| App       | URL                                                      |
| --------- | -------------------------------------------------------- |
| OpenWebUI | [http://your-server-ip:3002](http://your-server-ip:3002) |
| Flowise   | [http://your-server-ip:3003](http://your-server-ip:3003) |

> You can configure domains + HTTPS via Traefik, NGINX, or Cloudflare Tunnel.

---

## ⚙️ Config via `.env`

```env
OLLAMA_PORT=11434
OLLAMA_MODEL=llama3

INTERPRETER_MODEL=http://ollama:11434

OPENWEBUI_PORT=3002
FLOWISE_PORT=3003
```

---

## 📂 Folder Structure

```
snaredrop-ai-hub/
├── docker-compose.yml
├── .env.example
├── interpreter/             # Optional config for Open Interpreter
└── README.md
```

---

## 🛡 Security & Isolation

* All traffic is internal or via your reverse proxy
* No cloud APIs required (unless you choose to)
* Easily integrate with **Cloudflare**, **NGINX**, or **Coolify**

---

## 📖 Use Cases

* 🧠 Ask terminal questions & execute with Open Interpreter
* ✍️ Write code, blog posts, or support replies using OpenWebUI
* 🔌 Chain workflows visually with Flowise
* 🔍 Run fully local GPT-4-alternatives with Ollama

---

## 👨‍💻 Author

Made with 🔥 by [@freqkflag](https://github.com/freqkflag) aka **Joey King**
📍 Austin, TX
🕸️ [cultofjoey.com](https://cultofjoey.com) • [twist3dkinkst3r.com](https://twist3dkinkst3r.com)

---

## 🧪 Future Add-Ons

* [ ] PrivateGPT for querying local docs
* [ ] Supabase for memory/persistence
* [ ] Web terminal with LLM assistance
* [ ] VS Code integration
* [ ] Custom Ollama UIs (kinky/cyberpunk themes 😈)

---

## 🧠 License

This project is licensed under the **Cyberpunk Copyleft**.
Use it. Break it. Hack it. Just don’t gatekeep it.


