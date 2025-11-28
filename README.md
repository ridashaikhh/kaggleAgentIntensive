# Kaggle Agent Intensive - AI Dream Analyzer
## A modular multi-agent system for interpreting, understanding, and remembering dreams.
#### Notebook Link: kaggle.com/competitions/agents-intensive-capstone-project/writeups/new-writeup-1763657321824

### Overview:
This project contains the core logic for the AI Dream Analyzer Agent, a multi-agent system designed to help users understand and reflect upon their dreams. The system ingests free-text dreams, extracts symbolic and emotional content, generates interpretations, creates embeddings for long-term memory, stores results in a vector database, and supports memory-aware Q&A. Built with Gemini models, it shows how modular agents can work together to deliver psychological insight in a scalable way.

### Problem Statement:

- Dream interpretation is confusing, subjective, and easily forgotten. People wake up with:

- Fragmented dream memories

- Random symbols like water, dogs, roads, falling, running

- Strong emotions they cannot explain

- No understanding of patterns

- No system to store or search dreams later

- Dreams contain psychological insights, but most people have no tool to analyze them.

### Solution Statement:

This system automates dream analysis through structured agents.
Agents break the pipeline into clear components:

- Ingest text

- Clean the text

- Extract symbols

- Detect emotions

- Generate interpretations

- Create embeddings

- Store structured dream records

- Retrieve similar dreams later

This reduces mental effort while offering consistent, psychologically meaningful interpretations. Embeddings and vector search allow users to explore patterns across months of dreams, turning raw journaling into an intelligent, reflective experience.

### Architecture Overview:

The AI Dream Analyzer Agent is a multi-agent pipeline that:

- Takes a dream from the user

- Cleans the text

- Extracts symbols

- Detects emotions

- Generates interpretations

- Creates embeddings for long-term memory

- Stores all results in Supabase

- Supports memory-aware question answering

### Agents Included:

**Dream Ingest Agent** – Cleans and normalizes the raw dream text.

**Symbol Extraction Agent**– Identifies symbols, people, objects, places, and actions.

**Emotion Detection Agent** – Detects dominant and secondary emotions and emotional intensity.

**Emotion Detection Agent** – Detects dominant and secondary emotions and emotional intensity.

**Interpretation Agent** – Generates two interpretations and one reflective question.

**Embedding Agent** – Converts dreams into vector embeddings for semantic memory.

**Memory Storage Agent** – Saves the dream, symbols, emotions, interpretations, and embeddings in Supabase.

**Similarity Search Agent** – Retrieves past dreams that are semantically similar.

**Chat Agent** – Answers user questions using retrieved memories and produces insight-rich responses.

### Technologies Used:

- Gemini 2.5 Flash (reasoning)

- Gemini Embeddings (text-embedding-004)

- Supabase (vector storage)

- Python

- Strict JSON prompting for reliable outputs

Everything works together through one orchestrated pipeline.

### Conclusion:

The AI Dream Analyzer Agent demonstrates the power of modular multi-agent systems. By dividing the workflow into specialized agents, the system produces structured, meaningful dream insights. Raw dreams are transformed into symbolic, emotional, and interpretive layers, all preserved in long-term memory for future reflection. The architecture is reusable, extensible, and capable of growing into more advanced personal-insight tools.

### Future Improvements:

- Group dreams by recurring symbols

- Detect long-term psychological patterns

- Identify emotional cycles (fear → stress → relief)

- Auto-generate monthly dream summaries
