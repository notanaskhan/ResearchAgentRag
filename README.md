# ResearchAgentRag
This project showcases a fully local, privacy-preserving research assistant that leverages open-source LLMs, live internet search, and tool-augmented reasoning to deliver accurate, context-aware responses grounded in real-world data.

Built around the Mistral-7B-Instruct model and powered by the LangChain framework, the assistant mimics advanced multi-turn conversational behavior while dynamically retrieving and synthesizing external knowledge.

🌐 Key Features
Live Web Search: Retrieves relevant URLs using duckduckgo_search.DDGS, enabling the assistant to remain up-to-date with the latest online content.

Granular Content Processing: Uses WebBaseLoader to scrape online pages, then breaks them into semantically meaningful chunks via RecursiveCharacterTextSplitter.

Semantic Embeddings: Generates vector embeddings using all-MiniLM-L6-v2 (HuggingFace) and stores them in a local Chroma vector database for efficient similarity search.

Tool-Augmented Reasoning: Integrates a custom LangChain Tool() for semantic search over retrieved web content, allowing the agent to cite and reason with real sources.

Multi-Turn Conversational Agent: Powered by LangChain’s ConversationalReactDescription agent and ConversationBufferMemory, enabling memory retention and contextual dialogue flow.

Local LLM Inference: The Mistral-7B-Instruct model runs entirely on local hardware using the transformers.pipeline, ensuring full control over data privacy and cost.

🧩 Objectives & Capabilities
Simulate a responsive assistant that can search, retrieve, and synthesize live information.

Maintain conversation state and build context over multiple turns.

Provide responses that are both factually grounded and semantically relevant.

Demonstrate a cost-effective, self-hosted alternative to cloud LLM APIs like OpenAI’s.
