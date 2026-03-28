# MCP (Model Context Protocol)

## 📌 Overview

This content explains how MCP (Model Context Protocol) can be used to build an **AI-powered automated system**.

Example project: **Automatically creating an AI newsletter using AI agents + MCP**.

---

## 🚀 What is the Goal?

Problem:

* AI is growing very fast
* New tools, research, and updates come daily
* It is hard for students to stay updated

Solution:
👉 Build an **AI system that automatically creates a weekly newsletter**

---

## 💡 Key Idea

Use:

* AI (Claude)
* Multiple tools (Google Drive, GitHub, Web, etc.)
* MCP (to connect everything)

👉 Result: Fully automated pipeline

---

## 🧠 What is MCP (Simple Understanding)?

MCP helps:

* Connect AI with external tools
* Let AI use tools like a human

Example:

* AI can read Google Drive
* AI can search web
* AI can check emails

👉 Without writing heavy API code

---

## 🎯 Project Flow (Big Picture)

The system works in **3 phases**:

1. Research Phase
2. Editing Phase
3. Designing Phase

---

# 🧩 Phase 1: Research Phase

## Goal:

Collect all information needed for the newsletter

### Step 1: Decide Topics

AI checks:

* Content ideas (from Google Drive)
* Past performance data
* User feedback emails

👉 Then decides what topics to research

---

### Step 2: Do Research from Multiple Sources

AI uses tools via MCP:

* 🌐 Web → latest AI news
* 📄 arXiv → research papers
* 💻 GitHub → trending repos
* 🚀 Product Hunt → new AI tools
* 🐦 Twitter/X → trending discussions

---

### Step 3: Generate Research Files

AI creates **5 markdown files**:

Example:

```md
# Web Research
- Big story of the week
- Quick updates
```

Each source → one file

---

# 🧩 Phase 2: Editing Phase

## Goal:

Combine all research into a final draft

### Step:

AI:

* Reads all 5 research files
* Reads a sample newsletter template
* Combines everything

👉 Creates final structured newsletter

---

## 📰 Newsletter Structure (9 Sections)

1. Introduction
2. Big Story of the Week
3. Quick Updates
4. Research Papers
5. GitHub Repos
6. Learning Tutorial
7. AI Products
8. Tweets
9. Closing Notes

---

## Output:

```md
final_newsletter.md
```

---

# 🧩 Phase 3: Designing Phase

## Goal:

Convert draft into a professional email

### Step:

AI:

* Reads final markdown
* Applies design rules
* Generates HTML email

---

## Output:

* HTML Newsletter
* Plain text version (backup)

```html
newsletter.html
```

---

# ⚙️ Tools Used

Main AI:

* Claude

Connected tools via MCP:

* Google Drive
* Gmail
* Web Search
* GitHub
* arXiv
* Product Hunt
* Twitter
* Calendar

---

# 🔗 How MCP Works (Simple)

Instead of writing APIs manually:

You just write config like:

```json
{
  "tool": "github",
  "api_key": "your_key"
}
```

👉 MCP handles everything else

---

# ⚡ Key Benefits

* No heavy coding
* Easy tool integration
* Fully automated system
* Scalable workflow

---

# 🧪 Final Result

With just **3 prompts**, AI can:

1. Do research
2. Create content
3. Design newsletter

👉 End-to-end automation

---

# 🔥 Why This is Powerful?

* AI becomes more than chatbot
* Works like an **agent system**
* Can solve real-world problems

---

# 🧠 Key Learning

👉 MCP = Make AI more powerful by connecting tools

👉 AI Agents + MCP = Automation system

---

# 🚀 What You Can Build Using This Idea

* Auto blog generator
* AI research assistant
* Market analysis tool
* Social media content generator

---

# 📝 Conclusion

MCP is a powerful technology that:

* Connects AI with tools
* Automates workflows
* Reduces coding effort

👉 Learning MCP can help you build real-world AI systems

---

# 📌 Next Steps

To go deeper, learn:

* MCP architecture
* MCP servers & clients
* Building your own MCP tools

# 📘 Model Context Protocol (MCP) 

---

## 🚀 1. Introduction

This document explains **Model Context Protocol (MCP)** in very simple English with deep understanding.

MCP is becoming very popular and may become an **industry standard in the next 3–5 years**. fileciteturn0file0

---

## 🤖 2. Arrival of LLMs (ChatGPT Revolution)

* ChatGPT launched on **30 Nov 2022**
* 1 million users in 5 days
* 100 million users in 2 months fileciteturn0file0

### 💡 What changed?

Earlier:

* Humans → Machines (buttons, commands)
* Interaction was **transactional**

Now:

* Humans ↔ AI (natural language)
* Interaction is **conversational**

👉 You can talk to AI like a human.

---

## 🌊 3. Three Waves of AI Adoption

### 1️⃣ Wave 1: Curiosity Phase

* People asked fun/random questions
* Example:

  * "Explain physics like a cat"
  * "Write song about pizza"

👉 Goal: Explore AI

---

### 2️⃣ Wave 2: Professional Use

People started using AI for real work:

* Lawyers → summarize contracts
* Developers → debug code
* Teachers → create curriculum

👉 Result: **Productivity increased**

---

### 3️⃣ Wave 3: API Revolution

* Companies started integrating AI in software
* Examples:

  * MS Word, Excel → Copilot
  * Google Docs, Gmail → AI features

👉 AI became **everywhere**

---

## ⚠️ 4. Problem: Fragmentation

Now many AI tools exist:

* Notion AI
* Slack AI
* VS Code AI
* ChatGPT

### ❌ Problem:

These tools **do not talk to each other**

👉 Result:

* Information is scattered
* You must switch tools again and again

---

## 🎯 5. Vision vs Reality

### Vision:

One **Unified AI Agent** that:

* Understands all your work
* Solves everything

### Reality:

* Multiple AI tools
* No connection between them

👉 Main challenge = **Context Problem**

---

## 🧠 6. What is Context?

### Simple Definition:

> Context = All information AI can see while generating answer fileciteturn0file0

### Example:

If you ask:

1. What is Quantum Physics?
2. Is it difficult?

👉 AI understands question 2 using previous conversation

➡️ That previous chat = **Context**

---

## 🔥 7. Real-World Context (Complex Case)

Example: Software Engineer building feature

Context exists in:

* Jira → task
* GitHub → code
* Database → schema
* Google Drive → docs
* Slack → discussions

👉 Context is **spread across tools**

---

## 😵 8. The Big Problem: Copy-Paste Hell

To use AI:

* Copy Jira → paste
* Copy code → paste
* Copy DB schema → paste
* Copy docs → paste

👉 Takes 20+ minutes just to ask 1 question

### ❌ Problems:

* Time waste
* Not scalable
* Humans become “manual API”

---

## ⚙️ 9. Solution Attempt: Function Calling

### Idea:

Let AI call functions (tools)

Example:

```python
load_file("abc.txt")
```

### How it works:

1. Provide functions to AI
2. AI chooses correct function
3. Function executes task

👉 AI can now **perform actions, not just chat**

---

## 🛠️ 10. Rise of Tools

Different tools created:

* Weather API
* Database queries
* GitHub access
* Web search

👉 AI connects with tools → fetch context automatically

---

## ✅ 11. Improvement with Tools

Now instead of copy-paste:

You say:

* "Fetch Jira ticket"
* "Get code from GitHub"

👉 AI collects context automatically

---

## 🚨 12. New Problem: Integration Hell

If:

* n chatbots
* m tools

👉 You need = **n × m integrations**

### Problems:

* Too much coding
* Hard maintenance
* Security issues
* High cost

---

## 💡 13. Final Solution: MCP (Model Context Protocol)

### Core Idea:

Standard way for AI and tools to communicate

---

## 🏗️ 14. MCP Architecture

### Two components:

1. **Client** → AI chatbot (ChatGPT, Cursor)
2. **Server** → Tools (GitHub, Slack, DB)

👉 Communication happens using MCP protocol

---

## 🔄 15. How MCP Works

* AI connects to servers
* Servers provide tools + data
* No manual coding needed in client

👉 Server does all heavy work

---

## ⚖️ 16. MCP vs Function Calling

| Feature     | Function Calling | MCP              |
| ----------- | ---------------- | ---------------- |
| Code needed | Yes              | No (client side) |
| Integration | Manual           | Standard         |
| Scalability | Poor             | High             |
| Maintenance | High             | Low              |

---

## 🎁 17. Benefits of MCP

### ✅ 1. Fewer Integrations

From:

* n × m → many integrations

To:

* m + n → much fewer

---

### ✅ 2. No Maintenance

* Server handles updates
* Client unchanged

---

### ✅ 3. Faster Development

* Connect directly to servers
* No need to build integrations

---

### ✅ 4. Better Security

* Central config (JSON)
* Easier to manage

---

## 🌍 18. Why MCP is Growing Fast

* AI tools support MCP
* Companies forced to adapt
* Ecosystem growing fast

👉 Likely future standard

---

## 🧠 Final Summary

* AI needs **context** to work properly
* Context is scattered across tools
* Tools solved it partially
* But created integration problem

👉 MCP solves this by:

* Standardizing communication
* Reducing complexity
* Making AI truly powerful

---

## 📌 Key Takeaway

> MCP = Bridge between AI and real-world tools

---

## 🔚 End

These notes are based on the provided content and simplified deeply for understanding. fileciteturn0file0
# 📘 Model Context Protocol (MCP) — Part 1 (Architecture)

---

## 🧠 What is MCP?

![MCP Architecture](https://mcpcat.io/images/blog/mcp-architecture.png)
![Overview](https://miro.medium.com/v2/resize\:fit:1400/1-MfI2XLk63rQye0Sh-hAUag.png)

MCP (Model Context Protocol) is a standard that allows AI applications (like chatbots) to connect with external tools, data, and services.

👉 Simple idea:
**MCP = "USB port for AI" → connect AI to tools like GitHub, Slack, Database**

---

## 🧩 Basic MCP Architecture (Simplest Version)

![Basic Flow](https://media2.dev.to/dynamic/image/width=800/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/7lr9tmc9rnl5f96coirf.png)

### Components:

* Host (AI Chatbot)
* Server (Tool provider)

---

### 🔹 Host (AI Chatbot)

* User interacts with this
* Connected to LLM (OpenAI, Gemini, Claude)

### 🔹 Server (Tool)

* Performs actual tasks
* Examples:

  * GitHub → commits
  * Slack → messages
  * Drive → files

---

## 🔁 Simple Flow

1. User asks question
2. Host → LLM
3. LLM needs external data
4. Host → Server
5. Server → data
6. LLM → final answer

---

## ⚠️ Refined Architecture (Important)

👉 Host does NOT directly talk to Server

### New Component:

* Client (MCP Client)

---

## 🧩 Final Architecture

![Architecture](https://miro.medium.com/v2/resize\:fit:1200/1-hxvZY7Rg6hPKv8amieddOw.png)
![System Design](https://guptadeepak.com/content/images/size/w2000/2025/05/MCP-Architecture-Diagram---guptadeepak.com.png)

### Components:

* Host
* Client
* Server

---

## 🔹 Role of Client

![Client Role](https://media.springernature.com/lw1200/springer-static/image/art%3A10.1007%2Fs44163-024-00134-3/MediaObjects/44163_2024_134_Fig2_HTML.png)

* Acts as translator
* Converts request → MCP format
* Converts response → Host format

👉 Client speaks MCP language (JSON-RPC)

---

## 🔁 Updated Flow

1. User → Host
2. Host → Client
3. Client → Server
4. Server → Client
5. Client → Host
6. Host → User

---

## 🔗 Relationship Rule

👉 One Client ↔ One Server

* More servers = more clients

---

## 📱 Real-Life Analogy

![Analogy](https://www.altexsoft.com/media/2020/05/word-image-54.png)

| Real World | MCP    |
| ---------- | ------ |
| Phone      | Host   |
| SIM        | Client |
| Network    | Server |

---

## 🚀 Benefits

![Benefits](https://substackcdn.com/image/fetch/$s_!cv8k!,f_auto,q_auto\:good,fl_progressive\:steep/https://substack-post-media.s3.amazonaws.com/public/images/362128ff-7821-482e-b08a-8252d0faab99_1200x1200.png)

### 1. Decoupling

* Independent systems

### 2. Parallel Processing

* Multiple tasks at same time

### 3. Scalability

* Add unlimited servers

---

## 🧱 MCP Primitives

👉 What server offers to host

### 🔹 1. Tools

![Tools](https://www.altexsoft.com/media/2019/10/word-image-9.png)

* Actions
* Dynamic data

Examples:

* Create issue
* Get commits

---

### 🔹 2. Resources

![Resources](https://cdn.bulldogjob.com/system/photos/files/000/003/440/original/readme.png)

* Static data

Examples:

* README
* Database schema

---

### 🔹 3. Prompts

![Prompts](https://docs.github.com/assets/cb-80496/images/help/repository/sample-issue-form.png)

* Guidelines for AI

Example structure:

```
Title
Steps to reproduce
Expected behavior
Actual behavior
Environment
```

---

## ⚙️ Standard Operations

### Tools

* tools/list
* tools/call

### Resources

* resources/list
* resources/read
* subscribe/unsubscribe

### Prompts

* prompts/list
* prompts/get

---

## 🧠 Data Layer

![JSON RPC](https://opsi.org/en/blog/opsi-cli-jsonrpc/header.jpg)

👉 Language of MCP

* Uses JSON-RPC 2.0

---

## 🔗 JSON-RPC Example

```json
{
  "jsonrpc": "2.0",
  "method": "get_commits",
  "params": {
    "repo": "my-repo"
  },
  "id": 1
}
```

---

## 🔥 Final Summary

* MCP connects AI with tools
* Architecture: Host → Client → Server
* One client per server
* Server provides:

  * Tools
  * Resources
  * Prompts
* Uses JSON-RPC

---

## 🎯 Use Cases

* AI agents
* Automation systems
* Dev tools integration

---

## 📌 Source
# 📘 Model Context Protocol (MCP) — Part 2 (Data Layer + Transport Layer)

---

## 🧠 What is Data Layer?

![Data Layer](https://opsi.org/en/blog/opsi-cli-jsonrpc/header.jpg)
![JSON Structure](https://cdn.prod.website-files.com/5ff66329429d880392f6cba2/676ff01bb48efc129a28b29d_61b76e7fdf48bbef0026f39a_JSON%2520works.png)

👉 Data Layer = Language used for communication between Client and Server

* Defines rules (grammar)
* Defines structure of messages

📌 In MCP → Data Layer uses **JSON-RPC 2.0**

---

## 🔗 What is RPC?

![RPC](https://www.altexsoft.com/media/2020/05/word-image-54.png)

👉 RPC = Remote Procedure Call

Simple meaning:

> Call a function on another machine like it's local

Example:

Instead of:

```
add(2, 3)
```

You send request:

```
Run "add" with parameters 2 and 3
```

---

## 🔗 What is JSON-RPC?

![JSON RPC Flow](https://www.researchgate.net/publication/320078730/figure/fig5/AS%3A543639655141377%401506625202361/An-example-of-JSON-RPC-response.png)

👉 JSON-RPC = RPC + JSON format

* RPC → calling remote functions
* JSON → structure of message

---

## 🧾 JSON-RPC Request Structure

```json
{
  "jsonrpc": "2.0",
  "method": "add",
  "params": {
    "a": 2,
    "b": 3
  },
  "id": 1
}
```

### Explanation:

* `jsonrpc` → version
* `method` → function name
* `params` → inputs
* `id` → match request & response

---

## 🧾 JSON-RPC Response

```json
{
  "jsonrpc": "2.0",
  "result": 5,
  "id": 1
}
```

---

## ❌ Error Response

```json
{
  "jsonrpc": "2.0",
  "error": {
    "code": -32601,
    "message": "Method not found"
  },
  "id": 1
}
```

---

## ⚡ JSON-RPC in MCP (Important)

👉 All communication between Client & Server uses JSON-RPC

Example:

### tools/list

```json
{
  "jsonrpc": "2.0",
  "method": "tools/list",
  "id": 1
}
```

### tools/call

```json
{
  "jsonrpc": "2.0",
  "method": "tools/call",
  "params": {
    "name": "list_issues"
  },
  "id": 2
}
```

---

## 🔥 Advanced Features of JSON-RPC

### 1. Batch Requests

![Batch](https://substackcdn.com/image/fetch/$s_!cv8k!,f_auto,q_auto\:good,fl_progressive\:steep/https://substack-post-media.s3.amazonaws.com/public/images/362128ff-7821-482e-b08a-8252d0faab99_1200x1200.png)

👉 Send multiple requests at once

---

### 2. Notifications

👉 No response required

* Fire and forget
* No `id` field

---

## 🚀 Why JSON-RPC over REST?

| Feature      | JSON-RPC | REST          |
| ------------ | -------- | ------------- |
| Endpoint     | Single   | Multiple URLs |
| Format       | JSON     | JSON/XML      |
| Overhead     | Low      | High          |
| Batch        | Yes      | No            |
| Notification | Yes      | No            |

---

## 🧠 Transport Layer

![Transport](https://media.springernature.com/lw1200/springer-static/image/art%3A10.1007%2Fs44163-024-00134-3/MediaObjects/44163_2024_134_Fig2_HTML.png)

👉 Transport Layer = How messages travel

* Moves JSON-RPC messages
* Client ↔ Server communication medium

---

## 🔀 Types of Servers

### 1. Local Server

![Local](https://miro.medium.com/v2/resize\:fit:1200/1-5gFJX9g0nVddOZXS6AMDDA.png)

* Runs on same machine
* Example: file system access

---

### 2. Remote Server

![Remote](https://miro.medium.com/v2/resize\:fit:1400/1-6Xn1NsZM3Rp3XIanFkFJxQ.png)

* Runs on internet
* Example: GitHub API

---

## ⚙️ Transport for Local Server → STDIO

![STDIO](https://media.geeksforgeeks.org/wp-content/uploads/20240206154107/Standard-Input-Output.webp)

👉 STDIO = Standard Input Output

### How it works:

1. Host starts server as subprocess
2. Host sends data via stdin
3. Server sends response via stdout

---

## 💡 Example (Python)

```python
name = input("Enter name: ")
print("Hello", name)
```

👉 Input → stdin
👉 Output → stdout

---

## 🚀 Benefits of STDIO

* ⚡ Fast (same machine)
* 🔒 Secure (no network)
* 🧩 Simple implementation

---

## 🌐 Transport for Remote Server → HTTP + SSE

![HTTP](https://www.altexsoft.com/media/2020/05/word-image-54.png)
![SSE](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events/streaming.png)

### HTTP

* Used to send requests
* Uses POST request
* JSON payload

---

### SSE (Server-Sent Events)

👉 Used for streaming responses

* Server sends data continuously
* One connection, multiple messages

---

## 🔥 Why SSE?

* Real-time updates
* Streaming AI responses
* Long-running tasks

---

## 🧠 Important Concept

👉 JSON-RPC is **transport-agnostic**

Means:

* Works with STDIO
* Works with HTTP
* Works with WebSockets

---

## 🔥 Final Summary

* Data Layer → JSON-RPC
* Transport Layer → message delivery

### Local Server:

* Uses STDIO

### Remote Server:

* Uses HTTP + SSE

---

## 🎯 Key Insight

👉 MCP separates:

* Data Layer (language)
* Transport Layer (delivery)

➡️ This makes system flexible and scalable

---

## 📌 Source

Based on video content: fileciteturn1file0

