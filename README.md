🧠 MyMind

A private, retrieval-augmented AI assistant that turns your notes, PDFs, and documents into a searchable personal memory.

MyMind lets you upload documents, store them as semantic embeddings, and ask natural-language questions.
It retrieves relevant context and generates cited, synthesized answers — a personal-scale version of Glean.

🚀 Features
- 📄 Upload & Index PDFs – Extracts and embeds document text
- 🔍 Semantic Search – Finds information by meaning, not keyword
- 💬 Conversational Q&A – Answers with citations from your data
- 🧠 Persistent Memory – Keeps long-term context and history
- ☁️ Cloud-Ready – Deployable on Vercel + Cloud Run
- 🔐 Private – Data stored in your own Supabase instance

🔄 Core Flow
User → Upload PDF → Extract Text → Chunk + Embed
       ↓
Vector DB (Supabase/Pinecone) ← Store embeddings + metadata
       ↓
Query → Embed → Retrieve similar chunks → LLM synthesis → Answer + Sources

🧭 Roadmap
- Local RAG prototype
- FastAPI backend + Supabase vector DB
- Next.js chat interface
- Add Google Drive / Gmail connectors
- Personalized daily summaries
- Mobile & browser extensions

🧩 Example Query
User: Summarize everything I wrote about my Epic Systems internship.
Assistant: Your Epic project focused on a MyChart login-alert system...
Sources: [Epic_Report.pdf, Internship_Reflection.txt]

🧾 Summary
MyMind is a personal AI knowledge base built with a full RAG pipeline —
FastAPI backend, Supabase vector memory, and a Next.js chat UI.
It’s your own context-aware digital assistant, privately hosted and extensible.
