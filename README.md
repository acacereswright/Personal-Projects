# Personal Projects

A running list of ML/AI projects focused on learning by building. A secondary goal is to learn how to vibe code effectively.

## Projects

| # | Project | Category | Key Skills | Status |
|---|---------|----------|------------|--------|
| 1 | [Chat With Your Notes](https://github.com/acacereswright/chat-with-notes) | NLP / RAG | Embeddings, vector search, RAG architecture, document parsing | In Progress |
| 2 | Book Recommendation System | RecSys | Web scraping, recommendation algorithms, API integration | Planned |
| 3 | Custom Image Classifier | Computer Vision | Data collection, labeling, CNN training, model deployment | Planned |
| 4 | Sentiment Analysis Dashboard | NLP / Data Viz | API scraping, sentiment models, fine-tuning, visualization | Planned |
| 5 | Personal AI Coding Assistant | Code / Fine-tuning | Fine-tuning, code models, training data curation | Planned |
| 6 | Music/Podcast Recommendation Engine | RecSys | Collaborative filtering, content-based filtering, Spotify API | Planned |
| 7 | RL Agent for Game Playing | Reinforcement Learning | Reward shaping, policy gradients, Q-learning | Planned |
| 8 | ML-Powered Finance Categorizer | Tabular ML | Text classification, anomaly detection, dashboarding | Planned |
| 9 | Text-to-Image Prompt Optimizer | NLP / Generative AI | Fine-tuning, dataset creation, prompt engineering | Planned |

## Detailed Descriptions

---

### 1. Chat With Your Notes — Local RAG Study Tool

**Core idea:** Index your own notes into a vector DB and chat with them using a local LLM.

**Data sources (tiered by comfort level):**

| Tier | Scope | Description |
|------|-------|-------------|
| Tier 1 | No hesitation | Your own handwritten/typed notes, summaries, and assignments |
| Tier 2 | Local-only | Professor slides and textbook chapters — kept fully local, never hosted or shared |
| Tier 3 | Lighter touch | Only index your annotations/highlights from course materials, not the full text |

**Formats to support:** Markdown, PDF, PowerPoint/slides

**Components:**
- Document ingestion pipeline (parsing, chunking strategy)
- Embedding model (e.g., sentence-transformers or a small local model)
- Vector database (e.g., ChromaDB, FAISS, or LanceDB for local-first)
- Chat interface (start as CLI, evolve to a simple web UI)
- Local LLM for generation (e.g., Ollama with Llama/Mistral)

**Extension — "Help me plan papers" mode:**
- Search your notes for relevant material given a topic or prompt
- Generate outlines, identify which notes support each section, and flag gaps needing more research
- Suggest structure based on your past writing style if you feed in previous papers

---

### 2. Book Recommendation System

**Core idea:** Start as a book tracker and evolve into a recommendation engine.

- Build a tracker for books read, ratings, and notes
- Integrate with Goodreads or author pages via web scraping/APIs to pull in related books, other works by the same author, etc.
- Layer in recommendation logic over time (content-based, collaborative filtering)

---

### 3. Custom Image Classifier

**Core idea:** Train an image classifier on a dataset you collect yourself.

- Pick a niche domain (e.g., plant species in your area, dog breeds, food dishes)
- Practice the full loop: data collection, labeling, training, evaluation, and deployment as a simple web app

---

### 4. Sentiment Analysis Dashboard

**Core idea:** Build a dashboard that tracks sentiment trends for a subreddit or Twitter/X topic.

- Scrape or use APIs to collect posts
- Run sentiment models and visualize trends over time
- Explore both pre-trained models (HuggingFace) and fine-tuning your own

---

### 5. Personal AI Coding Assistant

**Core idea:** Fine-tune a code model on your own coding style.

- Collect your GitHub commits/PRs as training data
- Fine-tune a small code model (e.g., CodeLlama, StarCoder) to suggest completions in your style

---

### 6. Music/Podcast Recommendation Engine

**Core idea:** Build a recommendation engine using your own listening history.

- Pull listening data via the Spotify API
- Compare content-based vs. collaborative filtering approaches

---

### 7. RL Agent for Game Playing

**Core idea:** Train a small reinforcement learning agent to play a simple game.

- Start with something like CartPole or a grid world
- Progress to Atari or a custom environment

---

### 8. ML-Powered Personal Finance Categorizer

**Core idea:** Auto-categorize bank transactions using ML.

- Import bank transactions (CSV) and train a model to categorize spending
- Evolve into a budgeting dashboard with anomaly detection for unusual charges

---

### 9. Text-to-Image Prompt Optimizer

**Core idea:** Fine-tune a model to rewrite vague prompts into detailed ones that produce better results with Stable Diffusion / DALL-E.

- Build a dataset by pairing simple prompts with their improved versions
- Train a small model to perform the rewriting
