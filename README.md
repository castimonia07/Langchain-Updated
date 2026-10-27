# 🧠 Learning LangChain (Hands-on Notes & Experiments)

A personal learning repository and playground dedicated to exploring modern **LangChain** features, concepts, and patterns through practical Jupyter notebooks.

> 📝 **Note:** This is a personal study space and reference guide, not a production application or library. It contains code snippets, experiments, and conceptual breakdowns created while learning and practicing LangChain.

---

## 📚 What's Covered Here

All core study material and experiments live inside the [`updatedlangchain/`](./updatedlangchain/) directory:

| Notebook | Focus Area | Key Concepts Explored |
| :--- | :--- | :--- |
| **[`langchainintro.ipynb`](./updatedlangchain/langchainintro.ipynb)** | **LangChain Basics & Overview** | Introduction to modern LangChain architecture, agent concepts, and foundational workflows. |
| **[`modelintegration.ipynb`](./updatedlangchain/modelintegration.ipynb)** | **Multi-Provider Integrations** | Connecting and configuring various LLMs (OpenAI, Google Gemini, Groq, Ollama), batch invocations, and real-time response streaming. |
| **[`messages.ipynb`](./updatedlangchain/messages.ipynb)** | **Prompts & Message Architecture** | Difference between plain text prompts and message objects, message roles (`SystemMessage`, `HumanMessage`, `AIMessage`), multimodal inputs, and context management. |
| **[`structuredoutput.ipynb`](./updatedlangchain/structuredoutput.ipynb)** | **Structured & Schema-Enforced Outputs** | Extracting reliable, typed data using **Pydantic** models, nested structures, field validations, and inspecting raw outputs alongside parsed objects. |
| **[`tools.ipynb`](./updatedlangchain/tools.ipynb)** | **Tools & Function Calling** | Defining custom tools, binding tools to models, handling tool call invocations, and building agentic execution loops. |
| **[`Middleware.ipynb`](./updatedlangchain/Middleware.ipynb)** | **Agent Control & Middleware** | Managing agent execution flow, tracking intermediate states, and token-saving strategies like **Summarization Middleware** to compact long conversation histories. |

---

## 🛠️ Setup & Prerequisites

### 1. Environment Setup

Clone or open this folder in your IDE, then set up a virtual environment (using `uv` or standard `venv`):

```bash
# Using standard venv
python -m venv .venv

# On Windows (PowerShell):
.venv\Scripts\Activate.ps1

# On Linux/macOS:
source .venv/bin/activate
```

### 2. Install Dependencies

Install the required packages listed in `requirements.txt`:

```bash
pip install -r requirements.txt
```

Key packages used:
- `langchain` & `langchain-community`
- Provider integrations: `langchain-openai`, `langchain-google-genai`, `langchain-groq`, `langchain-ollama`
- `ipykernel` (to run the notebooks in VS Code or Jupyter Lab)
- `python-dotenv` & `pydantic`

### 3. API Keys Configuration

Create a `.env` file in the root directory and add the keys for the models you want to experiment with:

```env
OPENAI_API_KEY="your-openai-api-key"
GROQ_API_KEY="your-groq-api-key"
GOOGLE_API_KEY="your-google-gemini-api-key"
```

---

## 🎯 Learning Goals & Takeaways

- [x] Understand how modern LangChain abstracts LLM interfaces across different providers.
- [x] Master message flow (`HumanMessage` / `SystemMessage` / `AIMessage`) vs. raw string prompts.
- [x] Consistently extract structured data using Pydantic schemas.
- [x] Equip models with external capabilities using tools and execution loops.
- [x] Tame token limits with middleware and history summarization techniques.

---

## 📌 Helpful References

- [LangChain Official Documentation](https://python.langchain.com/)
- [LangChain Conceptual Guides](https://python.langchain.com/docs/concepts/)
- [Pydantic Documentation](https://docs.pydantic.dev/)
