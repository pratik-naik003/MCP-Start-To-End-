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

# MCP Lifecycle – Simple English Notes (Detailed)

---

## 📌 Introduction

This document explains the **MCP Lifecycle** in very simple English with full detail and examples.

👉 MCP Lifecycle means how **Client and Server connect, communicate, and disconnect** step by step.

---

## 🧠 What is MCP Lifecycle?

**Definition:**
MCP Lifecycle is the **complete sequence of steps** that explains how:

* Connection is created
* Communication happens
* Connection ends

📌 fileciteturn0file0

---

## 🔗 What is a Session?

A **session** is a continuous connection between:

* Client (Host)
* Server

### Example:

* Claude Desktop = Client
* GitHub MCP Server = Server

👉 When you start Claude Desktop:

* It connects to server automatically
* Connection stays active until you close it

That continuous connection = **Session**

---

## 🔄 MCP Lifecycle Phases

There are **3 main phases**:

1. Initialization Phase
2. Operation Phase
3. Shutdown Phase

---

# 🟢 1. Initialization Phase (Handshake Phase)

👉 This is the **first interaction** between client and server.

### Purpose:

* Check compatibility
* Exchange capabilities
* Establish connection

---

## ⚙️ Step-by-Step Process

### 🔹 Step 1: Client → Server (Initialize Request)

Client sends a request to server:

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "initialize",
  "params": {
    "protocolVersion": "2024-11-05",
    "capabilities": {
      "roots": {},
      "sampling": {}
    },
    "clientInfo": {
      "name": "client-app",
      "version": "1.0.0"
    }
  }
}
```

### 📌 What client sends:

* Protocol version
* Capabilities (what it can do)
* Client info

---

### 🔹 Step 2: Server → Client (Response)

Server replies with:

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "result": {
    "protocolVersion": "2024-10-01",
    "capabilities": {
      "tools": {},
      "resources": {}
    },
    "serverInfo": {
      "name": "filesystem-server",
      "version": "2.0.0"
    }
  }
}
```

### 📌 What server sends:

* Protocol version
* Capabilities
* Server info

---

### 🔹 Step 3: Client → Server (Initialized Notification)

```json
{
  "jsonrpc": "2.0",
  "method": "initialized"
}
```

👉 This means:

* Connection is successful
* Communication can start

---

## ⚠️ Important Rules

### Rule 1:

Client cannot send other requests before initialization completes

### Rule 2:

Server also cannot respond with other data before "initialized"

👉 Only allowed:

* Ping
* Logs

---

# 🔄 Version Negotiation

👉 What if versions are different?

### Process:

1. Client checks server version
2. Compares with supported versions
3. If supported → continue
4. If not → disconnect

---

# 🤝 Capability Negotiation

👉 Client and server tell each other:
**"What I can do"**

---

## 🧩 Client Capabilities

### 1. Roots

* Give access to file system

### 2. Sampling

* Server can use client’s AI

### 3. Elicitation

* Server asks for missing info

---

## 🧩 Server Capabilities

### 1. Tools

* Functions that client can use

### 2. Resources

* Static data (files/docs)

### 3. Prompts

* Instructions/templates

### 4. Logging

* Send updates during long tasks

---

## 🔔 Sub-Capabilities

### 1. list_changed

* Notify when tools/resources change

### 2. subscribe

* Get updates when resource changes

---

# 🟡 2. Operation Phase

👉 This is the **main working phase**

### What happens:

* Client sends requests
* Server processes them
* Server sends responses

---

## Example Request

```json
{
  "jsonrpc": "2.0",
  "id": 2,
  "method": "tools.call",
  "params": {
    "name": "createFile",
    "arguments": {
      "path": "test.txt"
    }
  }
}
```

---

## Rules:

* Use agreed protocol version
* Use only negotiated capabilities

---

# 🔴 3. Shutdown Phase

👉 Ending the session

### When happens:

* Client closes app
* Server stops

---

## Example

```json
{
  "jsonrpc": "2.0",
  "method": "shutdown"
}
```

---

# 💻 Practical Understanding

👉 Example setup:

* Client: Claude Desktop
* Server: File System MCP Server

### What server can do:

* Read files
* Create files
* Modify files

---

## 🧠 Key Takeaways

* MCP works in **3 phases**
* Initialization = handshake
* Operation = real work
* Shutdown = connection end
* JSON-RPC is used for communication

---

## 🚀 Final Summary

MCP Lifecycle =

1. Connect (Initialization)
2. Communicate (Operation)
3. Disconnect (Shutdown)

---

✔ This lifecycle is very important for building:

* MCP Servers
* MCP Clients
* AI Agent Systems

---

🔥 Now you are ready to implement MCP in real projects!


# MCP Lifecycle – Part 2 (Simple English Notes with Code)

---

## 📌 Introduction

This part explains the **Operation Phase (deep)**, **Shutdown Phase**, and **Special Cases** in MCP.

📌 fileciteturn1file0

---

# 🟡 Operation Phase (Detailed)

👉 This phase is divided into **2 main parts**:

1. Capability Discovery
2. Tool Calling

---

## 🔍 1. Capability Discovery

👉 Client finds out:

* Which tools are available
* Which resources are available
* Which prompts are available

---

### 📤 Client Request (Tools List)

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "method": "tools/list"
}
```

---

### 📥 Server Response

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "result": {
    "tools": [
      {"name": "readFile"},
      {"name": "writeFile"},
      {"name": "createDirectory"}
    ]
  }
}
```

---

### 📌 Important Points

* Happens **automatically after initialization**
* Client sends multiple requests:

  * tools/list
  * resources/list
  * prompts/list

---

### ❌ Error Example (Method Not Found)

```json
{
  "jsonrpc": "2.0",
  "id": 2,
  "error": {
    "code": -32601,
    "message": "Method not found"
  }
}
```

👉 Happens when server doesn’t support that feature

---

## ⚙️ 2. Tool Calling

👉 After discovery, client selects the correct tool

---

### 📤 Request (Tool Call)

```json
{
  "jsonrpc": "2.0",
  "id": 3,
  "method": "tools/call",
  "params": {
    "name": "readFile",
    "arguments": {
      "path": "desktop/hello.py"
    }
  }
}
```

---

### 📥 Response

```json
{
  "jsonrpc": "2.0",
  "id": 3,
  "result": {
    "content": "print('Hello World')"
  }
}
```

---

## 🧠 Flow Summary

1. User asks question
2. Client chooses tool
3. Server executes tool
4. Response returned

---

# 🔴 Shutdown Phase (Detailed)

👉 Ends the session between client and server

---

## 📌 Important Concept

* No JSON-RPC messages used
* Controlled by **transport layer**

---

## 🖥️ 1. Shutdown in STDIO (Local Server)

### ✔ Client Initiated (Common)

Steps:

1. Client closes input stream (stdin)
2. Waits for server to exit
3. If not → sends SIGTERM
4. If still not → sends SIGKILL

---

### ✔ Server Initiated (Rare)

* Server closes output stream
* Server exits

---

## 🌐 2. Shutdown in HTTP (Remote Server)

### ✔ Client Initiated

* Client closes HTTP connection

### ✔ Server Initiated

* Server drops connection
* Client must handle reconnect

---

# ⚡ Special Cases in MCP

---

## 📡 1. Ping

👉 Used to check if connection is alive

---

### 📤 Ping Request

```json
{
  "jsonrpc": "2.0",
  "id": 10,
  "method": "ping"
}
```

---

### 📥 Ping Response

```json
{
  "jsonrpc": "2.0",
  "id": 10,
  "result": {}
}
```

---

## 📌 When Used:

* During initialization
* During long operations
* Prevent connection drop

---

## ❗ 2. Error Handling

👉 MCP uses **JSON-RPC error format**

---

### 📦 Error Object

```json
{
  "jsonrpc": "2.0",
  "id": 5,
  "error": {
    "code": -32601,
    "message": "Method not found",
    "data": {}
  }
}
```

---

## 📌 Common Error Cases

* Version mismatch
* Invalid method
* Invalid arguments
* Server failure
* Timeout
* Invalid JSON

---

## 📊 Common Error Codes

| Code   | Meaning          |
| ------ | ---------------- |
| -32601 | Method not found |
| -32602 | Invalid params   |
| -32600 | Invalid request  |
| -32700 | Invalid JSON     |
| 32000+ | Server errors    |

---

## ⏳ 3. Timeout

👉 Prevents infinite waiting

---

### Flow:

1. Client sends request
2. Waits (e.g., 30 sec)
3. If no response → timeout
4. Cancel request

---

### 📤 Cancellation Notification

```json
{
  "jsonrpc": "2.0",
  "method": "notifications/cancelled",
  "params": {
    "requestId": 7,
    "reason": "timeout"
  }
}
```

---

## 📈 4. Progress Notification

👉 Used for long-running tasks

---

### 📤 Request with Token

```json
{
  "jsonrpc": "2.0",
  "id": 6,
  "method": "tools/call",
  "params": {
    "name": "scanRepo",
    "_meta": {
      "progressToken": "abc123"
    }
  }
}
```

---

### 📥 Progress Update

```json
{
  "jsonrpc": "2.0",
  "method": "notifications/progress",
  "params": {
    "progressToken": "abc123",
    "progress": 60,
    "message": "Scanning files..."
  }
}
```

---

## 📌 Benefits

* Better user experience
* Real-time updates
* No confusion during long tasks

---

# 🧠 Final Summary

### Operation Phase:

* Discover tools
* Call tools

### Shutdown Phase:

* Close connection

### Special Cases:

* Ping → check alive
* Errors → handle failures
* Timeout → stop waiting
* Progress → show updates

---

# 📘 MCP (Model Context Protocol) – Implementation Guide

## 📌 Introduction

This document explains how to **use MCP (Model Context Protocol)** in a practical way. MCP allows AI systems (like Claude Desktop) to connect with external tools and services.

---

## 🎯 Learning Plan

We learn MCP in 3 stages:

1. **Use Ready-made Tools**

   * Use existing MCP client (Claude Desktop)
   * Use existing MCP servers

2. **Build Your Own MCP Server**

   * Connect your custom server

3. **Build Your Own MCP Client**

   * Full control over communication

---

## 🧠 Core Concept

MCP works on **Client-Server Communication**:

* **Client (AI Host)** → Claude Desktop
* **Server** → Tools like File System, Google Drive, etc.

The client sends requests, and servers perform actions.

---

## ⚙️ Plan of Action

Steps:

1. Install Claude Desktop
2. Connect multiple MCP servers

### Servers Used:

* Local: File System, Manim
* Remote: Google Drive, Twitter, Weather

---

## 🌐 Types of MCP Servers

### 1. Local Server

* Runs on your computer
* Example: File System, Manim

### 2. Remote Server

* Runs on internet
* Example: Google Drive, APIs

---

## 🔗 Ways to Connect MCP Servers

### Method 1: JSON Configuration (Manual)

* Edit config file (JSON)
* Add server details manually
* Requires technical knowledge

### Method 2: Connectors (Easy Method)

* One-click connection
* No coding needed
* Handles authentication automatically

---

## 🔌 What are Connectors?

Connectors are built-in tools that connect AI to MCP servers automatically.

### Advantages:

* Easy to use
* No manual setup
* More secure
* Consistent performance

👉 Example: Like an **App Store for MCP tools**

---

## ❗ Why Not Use Connectors Always?

### Reason 1: Not Scalable

* Thousands of MCP servers exist
* Cannot build connectors for all

### Reason 2: MCP is Open Standard

* Anyone can create servers
* Forcing connectors would limit flexibility

👉 That’s why both methods exist.

---

## 💻 Step 1: Install Claude Desktop

1. Search: "Claude Desktop Download"
2. Install based on OS
3. Sign in

Interface is similar to ChatGPT.

---

## 📁 File System MCP Server

### Setup (Using Connector)

1. Open Claude Desktop
2. Go to Tools → Add Connectors
3. Install File System connector
4. Select accessible folders (e.g., Desktop)

### Features:

* Read files
* Create files
* Organize folders

### Example:

* Ask: "Find PDF files on my desktop"
* Ask: "Create Python file"

---

## 🎬 Manim MCP Server (Local Server)

### What is Manim?

* Python library for math animations
* Used by 3Blue1Brown

### What MCP Does:

* You write English prompt
* AI generates code
* Server creates animation video

### Setup Steps:

1. Install dependencies:

   ```bash
   pip install manim
   pip install mcp
   ```

2. Clone repository

3. Edit JSON config file

4. Add:

   * Python path
   * Manim executable path
   * Server file path

5. Restart Claude Desktop

### Example Prompt:

"Create animation of vector transformation"

👉 Output: Video visualization

---

## ☁️ Google Drive MCP Server

### Setup (Connector)

1. Click Tools
2. Connect Google Drive
3. Login with Google account

### Features:

* Read documents
* Summarize files

⚠️ Note: Read-only access

---

## 🐦 Twitter MCP Server

### Setup (JSON Method)

1. Get developer account
2. Generate API keys
3. Add to config file

### Features:

* Search tweets
* Post tweets (if permission enabled)

---

## 🌦️ Weather MCP Server (Remote)

### Setup:

1. Install uv:

   ```bash
   pip install uv
   ```

2. Get API key (AccuWeather)

3. Add config in JSON

4. Restart Claude

### Use:

* Ask: "Weather in Mumbai"

---

## 🔍 Finding MCP Servers

Search:
👉 "Awesome MCP Servers GitHub"

You will find:

* Categorized list
* Many useful tools

---

## 🚀 Key Takeaways

* MCP connects AI with tools
* Works via client-server model
* Two connection methods:

  * Connectors (easy)
  * JSON config (flexible)
* Can automate workflows
* Can build powerful AI systems

---

## 🎯 Final Advice

* Install Claude Desktop
* Try different MCP servers
* Build your own workflows
* Experiment and explore

👉 MCP is very powerful for automation and AI integration

# MCP (Model Context Protocol) – Simple Notes

## 📌 Overview

This content explains how to build your own **MCP server** using FastMCP.

The learning is divided into 3 parts:

* **Why MCP?** → Why we need it
* **What is MCP?** → Architecture + lifecycle
* **How to use MCP?** → Build servers and clients

👉 In this part, we focus on:

* Building a **local MCP server**
* Creating a real project: **Expense Tracker**

---

# 🧠 What is MCP?

MCP (Model Context Protocol) is a **set of rules (protocol)** that allows:

* LLMs (like Claude, ChatGPT)
* Tools (like DB, APIs)

to communicate with each other.

👉 Instead of writing complex integrations, MCP standardizes everything.

---

# ⚡ Problem Before MCP

Before MCP:

* Hard to connect AI with tools
* Repetitive code
* Complex integrations

---

# 🚀 Solution: MCP + Libraries

Instead of coding everything from scratch, we use libraries:

### 1. MCP SDK

* Official library
* Powerful but complex
* Lots of boilerplate code

### 2. FastMCP (Recommended ✅)

* Built on top of MCP SDK
* Simple and beginner-friendly
* Less code

👉 Think like:

* MCP SDK = TensorFlow
* FastMCP = Keras

---

# 📦 Installation Steps

## Step 1: Install UV (faster than pip)

```bash
pip install uv
```

## Step 2: Create Project Folder

```bash
mkdir expense-tracker-mcp
cd expense-tracker-mcp
```

## Step 3: Initialize Project

```bash
uv init .
```

## Step 4: Install FastMCP

```bash
uv add fastmcp
```

## Step 5: Check Installation

```bash
fastmcp version
```

---

# 🏗️ Basic MCP Server (Demo)

We create a simple server with 2 tools:

* Roll Dice 🎲
* Add Numbers ➕

## Code Example

```python
from fastmcp import FastMCP
import random

mcp = FastMCP("Demo Server")

@mcp.tool()
def roll_dice(n: int) -> list:
    return [random.randint(1, 6) for _ in range(n)]

@mcp.tool()
def add_numbers(a: int, b: int) -> int:
    return a + b

if __name__ == "__main__":
    mcp.run()
```

👉 Key Idea:

* `@mcp.tool()` → converts function into MCP tool
* `mcp.run()` → starts server

---

# 🧪 Testing Server (MCP Inspector)

Run this command:

```bash
uv run fastmcp dev main.py
```

👉 Opens MCP Inspector (like Postman for MCP)

You can:

* See tools
* Run tools
* Debug server

---

# ▶️ Running the Server

```bash
uv run fastmcp run main.py
```

---

# 🔗 Connect with Claude Desktop

```bash
uv run fastmcp install claude-desktop main.py
```

If error occurs:

* Replace `uv` with full path

---

# 💡 Main Project: Expense Tracker MCP Server

## Idea

Instead of using apps, you can say:

👉 "I spent ₹20 on milk"

And AI will:

* Add to database
* Track expenses
* Answer queries

---

# 🧩 Features

### 1. Add Expense

* Add transaction

### 2. List Expenses

* View all expenses

### 3. Summarize

* Total spending
* Category-wise analysis

---

# 🗄️ Database (SQLite)

We use SQLite (simple DB stored in file).

## Table Schema

* id
* date
* amount
* category
* subcategory
* note

---

# 🧾 Code: Initialize Database

```python
import sqlite3

conn = sqlite3.connect("expenses.db")
cursor = conn.cursor()

cursor.execute("""
CREATE TABLE IF NOT EXISTS expenses (
    id INTEGER PRIMARY KEY,
    date TEXT,
    amount REAL,
    category TEXT,
    subcategory TEXT,
    note TEXT
)
""")

conn.commit()
conn.close()
```

---

# ➕ Tool: Add Expense

```python
@mcp.tool()
def add_expense(date, amount, category, subcategory, note):
    conn = sqlite3.connect("expenses.db")
    cursor = conn.cursor()

    cursor.execute(
        "INSERT INTO expenses (date, amount, category, subcategory, note) VALUES (?, ?, ?, ?, ?)",
        (date, amount, category, subcategory, note)
    )

    conn.commit()
    conn.close()

    return "Expense added successfully"
```

---

# 📋 Tool: List Expenses

```python
@mcp.tool()
def list_expenses():
    conn = sqlite3.connect("expenses.db")
    cursor = conn.cursor()

    cursor.execute("SELECT * FROM expenses ORDER BY date ASC")
    rows = cursor.fetchall()

    conn.close()
    return rows
```

---

# 🔍 Improved Feature (Date Range)

```python
@mcp.tool()
def list_expenses(start_date, end_date):
    conn = sqlite3.connect("expenses.db")
    cursor = conn.cursor()

    cursor.execute(
        "SELECT * FROM expenses WHERE date BETWEEN ? AND ?",
        (start_date, end_date)
    )

    rows = cursor.fetchall()
    conn.close()

    return rows
```

---

# 🧠 Key Concepts

### MCP Components

* Tools → Functions
* Resources → Data
* Prompts → Instructions

### Transport

* Local: STDIO
* Remote: HTTP

---

# 🛣️ Roadmap

1. Build basic server ✅
2. Add features (expense tracker) ✅
3. Improve features (filters, summary)
4. Deploy as remote server
5. Build your own MCP client

---

# 💡 Extra Ideas

You can extend project:

* Edit expense
* Delete expense
* Add income
* Graph visualization

---

# 🎯 Final Understanding

MCP allows:

* Natural language → real actions
* AI → control tools

👉 Example:
"Show my last 7 days expenses"

AI will:

1. Understand query
2. Call MCP tool
3. Fetch data
4. Return result

---

# 📌 Conclusion

* MCP = future of AI tool integration
* FastMCP = easiest way to build MCP apps
* Start with local → move to remote

---
# Remote MCP Server (Simple Notes + Code)

## 📌 What is MCP?

MCP (Model Context Protocol) allows you to create servers that provide tools, resources, and data to AI models.

---

## 🏠 Local vs 🌐 Remote MCP Server

### Local MCP Server

* Runs on your own machine
* Faster (no internet communication)
* Only you can use it

### Remote MCP Server

* Runs on another machine (internet server)
* Can serve multiple users
* More powerful (better compute)
* Slightly slower (network delay)

👉 In real-world (companies), most MCP servers are **remote**.

---

## 🎯 Goal of This Project

We will:

1. Create a simple remote MCP server
2. Add tools (like add numbers, random number)
3. Deploy it online
4. Connect it with client (Claude Desktop)

---

## ⚙️ Step 1: Setup Environment

Install `uv`:

```bash
pip install uv
```

Create project folder:

```bash
mkdir test-remote-server
cd test-remote-server
```

Initialize project:

```bash
uv init .
```

Install FastMCP:

```bash
uv add fastmcp
```

---

## 🧠 Step 2: Basic MCP Server Code

Create `main.py` file:

```python
from fastmcp import FastMCP
import random

mcp = FastMCP("Simple Calculator Server")

# Tool 1: Add two numbers
@mcp.tool()
def add(a: int, b: int) -> int:
    return a + b

# Tool 2: Generate random number
@mcp.tool()
def random_number(min: int, max: int) -> int:
    return random.randint(min, max)

# Resource
@mcp.resource()
def server_info() -> str:
    return "This is a simple MCP server"

if __name__ == "__main__":
    mcp.run(
        transport="http",
        host="0.0.0.0",
        port=8000
    )
```

### 🔥 Important Change (Local → Remote)

* Local uses: `mcp.run()`
* Remote uses:

```python
mcp.run(transport="http", host="0.0.0.0", port=8000)
```

---

## ▶️ Step 3: Run Server

```bash
uv run main.py
```

---

## 🧪 Step 4: Test using MCP Inspector

```bash
uv run fastmcp dev main.py
```

* Select: `streamable-http`
* Click connect
* Test tools (add, random number)

---

## 🚀 Step 5: Deploy Server (FastMCP Cloud)

1. Push code to GitHub

```bash
git init
git add .
git commit -m "initial commit"
git remote add origin <repo-url>
git push origin main
```

2. Go to: [https://fastmcp.cloud](https://fastmcp.cloud)
3. Connect GitHub
4. Select repo
5. Deploy

👉 You will get a **public URL** for your MCP server.

---

## 🔗 Step 6: Connect to Claude Desktop

* Go to Settings → Connectors
* Add Custom Connector
* Paste server URL

⚠️ Note: Custom connector works only in **Pro plan**

---

## 🛠️ Free Plan Solution (Proxy Server)

If you don’t have Pro plan:

### Idea:

Claude → Local Proxy → Remote MCP Server

### Proxy Code:

```python
from fastmcp import FastMCP

mcp = FastMCP.as_proxy(
    "https://your-remote-server-url",
    name="Proxy Server"
)

if __name__ == "__main__":
    mcp.run()
```

Run:

```bash
uv run fastmcp install claude-desktop main.py
```

---

## ⚠️ Problems & Fixes

### 1. Database Read-Only Issue

* Happens after deployment
* Fix: Change DB handling (write-enabled path)

---

### 2. Blocking Server (Slow for multiple users)

Problem:

* One user blocks others

Solution:

* Use async programming

```bash
uv add aiosqlite
```

Example:

```python
import aiosqlite

async def add_expense():
    async with aiosqlite.connect("db.sqlite") as db:
        await db.execute("...")
```

---

### 3. Multi-user Problem (BIG ISSUE)

Problem:

* All users share same database
* No user identification

Solution:

* Add `user_id` in database
* Add authentication system

---

## 🧠 Key Learnings

* Remote MCP servers are future of AI tools
* Only transport changes (HTTP vs STDIO)
* Deployment makes your server public
* Async improves performance
* Authentication is important for real apps

---

## 🚀 Next Steps

* Build your own MCP client
* Learn authentication in MCP
* Add user sessions
* Explore advanced concepts:

  * Sampling
  * Elicitation

---

## ✅ Summary

You learned how to:

* Build MCP server
* Convert local → remote
* Deploy online
* Connect with client
* Handle real-world issues

---

💡 Tip: Try building your own project like:

* Expense tracker MCP
* Weather MCP
* College info MCP






