#  Celebrity Info AI Chatbot

A Streamlit-based conversational AI app that uses OpenAI's GPT models via LangChain to generate dynamic, context-aware responses about celebrities.

##  Features

-  **LangChain Integration**: Uses `LLMChain`, `PromptTemplate`, and `ConversationBufferMemory` for structured interactions.
-  **OpenAI GPT Models**: Generates intelligent responses using OpenAI’s language models.
-  **Streamlit UI**: Clean, interactive web interface for user input and real-time output.
-  **Modular Design**: Easily extendable with tools like Pinecone (vector DB), SerpAPI, or LangGraph.

## How It Works

1. User inputs a celebrity name.
2. The prompt template injects the input: `"Tell me about celebrity {name}"`.
3. LangChain sends the prompt to OpenAI GPT, retrieves a response.
4. The chatbot displays the response via Streamlit.

##  Tech Stack

- [LangChain](https://www.langchain.com/)
- [OpenAI API](https://platform.openai.com/)
- [Streamlit](https://streamlit.io/)
- Python 3.9+

##  Example Prompt

```python
PromptTemplate(
    input_variables=["name"],
    template="Tell me about celebrity {name}"
)
