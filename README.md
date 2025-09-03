# 📚 DocuSphere – The Modern, Modular GitBook Alternative

Welcome to **DocuSphere**, an open-source, extensible, and developer-friendly documentation platform designed to be integrated **at the code level** or **via APIs**.

Think **GitBook meets Notion**, but fully self-hostable, customizable, and built for teams that want full control over their docs and workflows.

> ⭐ Star this repository to help the project grow and attract contributors!
> 
[![OSCI-Project-Banner.png](https://i.postimg.cc/76mJvBmF/OSCI-Project-Banner.png)](https://postimg.cc/8JfzMb84)

---

## 🎯 Vision

DocuSphere empowers teams to:
- ✍️ Create **beautiful, structured documentation**
- 👥 **Collaborate in real-time** with role-based permissions
- 📦 Integrate **directly into your codebase**
- 🕓 Maintain **versioned content** for releases
- ⚡ Deliver **fast, searchable** reading experiences

---

## 🧩 Core Features

### **User Experience**
- 📂 **Sidebar Navigation** with drag-and-drop reordering
- 📝 **Markdown & Rich Text Editing**
- 📱 **Fully responsive** for mobile & desktop
- 🌗 **Dark/Light Theme Toggle**
- 🔍 **Fuzzy Search** across all docs
- 💬 Optional **per-page discussions/comments**
- 📌 **Pin favorite pages** for quick access

### **Editor & Admin Controls**
- 🖋 **Real-time collaborative editing**
- ♻️ **Auto-save with version history**
- 🗂 **Page & Folder Hierarchies**
- 📥 Import/Export **Markdown & JSON**
- 🔐 **Role-Based Access Control** (Admin, Editor, Viewer)
- ⏪ **One-click rollback** to older versions

### **Integration Capabilities**
- 📡 **REST & GraphQL APIs**
- 🧩 **Embed components directly in React/Next.js**
- 🔄 **Sync with GitHub repos** for docs-as-code workflows
- 🖇 **Link docs to other app modules** (projects, tasks, tickets)
- 🛠 **Plugin system** for extending features (search providers, export formats, etc.)

---

## 🧰 Tech Stack

| Layer        | Technology                          |
|--------------|-------------------------------------|
| Frontend     | React + Vite                        |
| Styling      | Tailwind CSS                        |
| Editor       | TipTap / Monaco / SimpleMDE         |
| Backend      | Node.js + Express                   |
| Database     | MongoDB                             |
| Auth         | JWT + RBAC                          |
| Real-time    | Socket.IO                           |
| Hosting      | Vercel / Render / Netlify           |

---

## 🗂 Suggested Folder Structure

```
/docusphere
├── client/               # Frontend
│   ├── components/
│   ├── pages/
│   ├── hooks/
│   ├── styles/
│   └── App.jsx
├── server/               # Backend
│   ├── models/
│   ├── controllers/
│   ├── routes/
│   ├── sockets/
│   └── server.js
├── shared/               # Shared utils/constants
├── plugins/              # Optional feature modules
├── .env.example
└── README.md
```

> This repository is a starter. All code and folders will be created through contributions and PRs.

---
🚀 Getting Started
1️⃣ Clone the Repo
git clone https://github.com/devayanm/docusphere
cd docusphere

2️⃣ Install Dependencies

Install backend and frontend dependencies separately:

# Backend
cd server
npm install

# Frontend
cd ../client
npm install


ℹ️ Note: There is no package.json at the root. Dependencies are managed individually inside server/ and client/.

3️⃣ Set Up Environment
# Copy example env file inside /server
cd server
cp .env.example .env
# Fill in required values: MONGODB_URI, JWT_SECRET, etc.

4️⃣ Start Development Servers
# Start backend (from /server)
npm run dev

# In a separate terminal, start frontend (from /client)
cd ../client
npm run dev
---

## 🤝 Contribution Guide

We welcome contributions of all sizes — from docs to major features.

### Workflow
1. **Fork** the repo
2. **Clone** your fork
3. Create a **feature branch** `git checkout -b feat/your-feature`
4. Commit & push
5. Open a **PR** and link related issues

### Commit Convention
Use [Conventional Commits](https://www.conventionalcommits.org/):
```
feat: add page version rollback
fix: resolve sidebar drag issue
docs: update README
```

---

## 📄 License
Released under the **MIT License**.
