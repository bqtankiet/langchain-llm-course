# LangChain for LLM Application Development
<a href="https://learn.deeplearning.ai/accomplishments/4d2cc912-7f7d-4d9e-9efb-1f7887247f2e?usp=sharing" target="_blank">
  Bùi Quang Tấn Kiệt, congratulations on completing LangChain for LLM Application Development!
  <img width="1088" height="196" alt="trello com_c_8684mj6V_25-langchain-for-llm-application-development" src="https://github.com/user-attachments/assets/7a8c0acf-a547-4181-8f50-7d7e14bfb128" />
</a>

### Lesson 1: Model, Prompts and Parser <a target="_blank" href="https://colab.research.google.com/github/bqtankiet/langchain-llm-course/blob/main/L1_Model_prompt_parser.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

- How to set up the environment: Installing necessary libraries like python-dotenv and langchain-groq, and managing API keys securely.
- How to interact with LLMs: Using init_chat_model to connect to a language model and send prompts.
- How to use Prompt Templates: Creating dynamic and reusable prompts with ChatPromptTemplate to guide the LLM's output.
- How to structure LLM output: Using StructuredOutputParser and ResponseSchema to get structured JSON data from the LLM.
- How to chain components with LCEL: Using the pipe operator (|) to create a clean and readable pipeline of operations.

### Lesson 2: Memory <a target="_blank" href="https://colab.research.google.com/github/bqtankiet/langchain-llm-course/blob/main/L2_Memory.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

- The Importance of Memory: I learned why memory is crucial for building conversational AI and how LLMs are inherently stateless.
- Manual Memory Implementation: I saw how to build a basic memory system from scratch using a simple Python list to store conversation history.
- Legacy LangChain Memory (Deprecated): I explored the now-deprecated memory modules in LangChain, such as `ConversationBufferMemory`, `ConversationBufferWindowMemory`, `ConversationTokenBufferMemory`, and `ConversationSummaryBufferMemory`, to understand the evolution of memory management.
- The Modern Approach with `RunnableWithMessageHistory`: I learned how to use the recommended `RunnableWithMessageHistory` to create stateful, session-aware conversational chains.
- Customizing Memory with `BaseChatMessageHistory`: I discovered how to create a custom memory class by inheriting from `BaseChatMessageHistory`, allowing for tailored memory management and summarization logic.

### Lesson 3: Chains <a target="_blank" href="https://colab.research.google.com/github/bqtankiet/langchain-llm-course/blob/main/L3_Chains.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

- How to create a simple chain with LangChain Expression Language (LCEL) using the | (pipe) operator.
- How to build a Sequential Chain where the output of one component becomes the input of the next.
- How to execute chains in parallel using `RunnableParallel` to create a Parallel Chain.
- How to implement a Router Chain with `RunnableBranch` to dynamically route inputs to different chains based on the input.

### Lessons 4: Q&A over Documents <a target="_blank" href="https://colab.research.google.com/github/bqtankiet/langchain-llm-course/blob/main/L4_QnA.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

- How to load and prepare document data for RAG (`CSVLoader`)
- How to embed documents using HuggingFace models
- How to create a vector store for semantic search
- How to manually construct a RAG pipeline using retrievers and LLMs
- How to simplify the full pipeline using `VectorstoreIndexCreator`

### Lesson 5: Evaluation <a target="_blank" href="https://colab.research.google.com/github/bqtankiet/langchain-llm-course/blob/main/L5_Evaluation.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

- **Manual Evaluation**: Use `set_debug(True)` and `set_verbose(True)` to check RAG outputs  
- **LLM Evaluation**: Use `QAEvalChain` to grade answers with an LLM  
- **Semantic Similarity**: Use sentence transformers + `cosine_similarity` to compare answers
