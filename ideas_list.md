# Personal Projects

This is a running list of personal projects that I want to complete at some point. I'm focusing on ML projects for now, but may expand. A secondary part is to learn how to vibe code effecitvly.

## Ideas

1. "Chat with your notes" — a local RAG-based study tool
	a. **Core idea**: Index your own notes into a vector DB and chat with them using a local LLM
	b. **Data sources (tiered by comfort level)**:
		- Tier 1 (no hesitation): Your own handwritten/typed notes, summaries, and assignments
		- Tier 2 (local-only): Professor slides and textbook chapters — kept fully local, never hosted or shared, used as a personal study aid
		- Tier 3 (lighter touch): Only index your annotations/highlights from course materials rather than the full text
	c. **Formats to support**: Markdown, PDF, PowerPoint/slides
	d. **Components**:
		- Document ingestion pipeline (parsing, chunking strategy)
		- Embedding model (e.g., sentence-transformers or a small local model)
		- Vector database (e.g., ChromaDB, FAISS, or LanceDB for local-first)
		- Chat interface (could start as CLI, evolve to a simple web UI)
		- Local LLM for generation (e.g., Ollama with Llama/Mistral)
	e. **Extension — "Help me plan papers" mode**:
		- Given a topic or prompt, the chatbot searches your notes for relevant material you've already studied
		- Helps generate outlines, identify which of your notes support each section, and flag gaps where you might need more research
		- Could suggest structure based on your past writing style if you feed in previous papers
	f. **Skills learned**: Embeddings, chunking strategies, vector search, RAG architecture, prompt engineering, document parsing
2. Build a recommendation system for books.
	a. Could stqart off as as a book tracker and build from there. I think something interesting could be to also do web calls or other things to get information fro mgood reads or the authors pages to learn about what other books they have
4. Train an image classifier on a custom dataset you collect yourself
	a. Pick a niche domain (e.g., plant species in your area, dog breeds, food dishes)
	b. Practice the full loop: data collection, labeling, training, evaluation, and deployment as a simple web app
5. Build a sentiment analysis dashboard for a subreddit or Twitter/X topic
	a. Scrape or use APIs to collect posts, run sentiment models, and visualize trends over time
	b. Could explore both pre-trained models (HuggingFace) and fine-tuning your own
6. Create a personal AI coding assistant fine-tuned on your own coding style
	a. Collect your GitHub commits/PRs as training data
	b. Fine-tune a small code model (e.g., CodeLlama, StarCoder) to suggest completions in your style
7. Build a music or podcast recommendation engine using collaborative filtering
	a. Use your own listening history (Spotify API) as the dataset
	b. Compare content-based vs. collaborative filtering approaches
8. Experiment with training a small RL agent to play a simple game
	a. Start with something like CartPole or a grid world, then move to Atari or a custom environment
	b. Good for learning reward shaping, policy gradients, and Q-learning hands-on
9. Build an ML-powered personal finance categorizer
	a. Import bank transactions (CSV) and train a model to auto-categorize spending
	b. Could evolve into a budgeting dashboard with anomaly detection for unusual charges
10. Create a text-to-image prompt optimizer
	a. Fine-tune a small model to rewrite vague prompts into detailed ones that produce better results with Stable Diffusion / DALL-E
	b. Build a dataset by pairing simple prompts with their improved versions
