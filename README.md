# LangChain 2: Working with LLMs and Groq

## How to run?

1. Create a new Python environment (recommended: conda):

   ```
   conda create -n llmapp python=3.11 -y
   conda activate llmapp
   ```

2. Install dependencies:

   ```
   pip install -r requirements.txt
   ```

3. Set your Groq API key in a `.env` file:
   ```
   GROQ_API_KEY=your_groq_api_key_here
   ```

## 🔧 Key Components

- **Environment Configuration:**  
  Loaded environment variables securely with `load_dotenv()` and `find_dotenv()` to manage the `GROQ_API_KEY`.

- **Model Setup:**  
  Integrated `langchain_groq` with `ChatGroq` to run high-performance LLM queries using `llama3-70b-8192`.

- **Prompt Engineering:**  
  Utilized `ChatPromptTemplate` and `FewShotChatMessagePromptTemplate` for efficient few-shot learning and contextual prompting.

- **Chaining Logic:**  
  Created a structured chain pipeline for input–output flow using the `|` operator to combine prompts, models, and output parsers.

- **Output Parsing:**  
  Used `SimpleJsonOutputParser` and `json_chain` to convert model responses into clean, structured JSON outputs.

## 📚 Topics Covered

### 1. Chat Completion Model

Demonstrates how to use `ChatGroq` with a chat prompt template for conversational AI tasks.

### 2. Prompt Templates

Shows how to build flexible prompts using `ChatPromptTemplate` for dynamic message formatting.

### 3. Few-Shot Prompting

Uses `FewShotChatMessagePromptTemplate` to provide the model with examples, improving response quality for tasks like translation or joke generation.

### 4. Chaining

Illustrates chaining prompts, models, and parsers for streamlined input-output processing.

### 5. Output Parsers

Explains how to parse LLM outputs into structured formats (like JSON) using `SimpleJsonOutputParser`.

### 6. Environment Management

Describes secure handling of API keys and environment variables using `python-dotenv`.

## 📦 Requirements

See `requirements.txt` for all dependencies, including:

- langchain
- langchain-groq
- python-dotenv

---

**Note:**  
Replace `your_groq_api_key_here` with your actual Groq API key in the `.env` file.  
For more details, see the
