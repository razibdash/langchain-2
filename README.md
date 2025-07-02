## How to run?

1. conda create -n llmapp python=3.11 -y

2. conda activate llmapp

3. pip install -r requirements.txt

## 🔧 Key Components:

<p>Environment Configuration: Loaded environment variables securely with load_dotenv() and find_dotenv() to manage the GROQ_API_KEY.</p>

<p>Model Setup: Integrated langchain_groq with ChatGroq to run high-performance LLM queries using llama3-70b-8192.</p>

<p>Prompt Engineering: Utilized ChatPromptTemplate and FewShotChatMessagePromptTemplate for efficient few-shot learning and contextual prompting.</p>

<p>Chaining Logic: Created a structured chain pipeline for input–output flow.</p>

<p>Output Parsing: Used SimpleJsonOutputParser and json_chain to convert model responses into clean, structured JSON outputs.</p>
