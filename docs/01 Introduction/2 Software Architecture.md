# 2| Software Architecture

Our software architecture for the Contoso Project integrates various technologies to deliver a robust and scalable chatbot application, including next.js, Python, Hugging Face, AI Studie, Prompt Flow, Azd CLI, Tailwind, AI search, and Cosmo DB. Below is an overview of the key components and their interactions within our system.

---

## System Overview

![Our Software Architecture](https://microsoft-contoso-group-project.github.io/website/img/SA_diagram.png)


## Key Components

1. **Chat Interface**:  
Accepts prompts from the retail website user in either text or audio format.
   
2. **Speech to Text Model**:  
If the prompt is in audio format, it is sent to a Whisper model on Hugging Face for transcription.
   
3. **Chat Function**:  
Acts as the "brain" of Contoso Chat, serving as the interface between Hugging Face models and Azure services.
   
4. **Embedding Model**:  
Converts incoming queries into multidimensional vectors to aid in semantic search.

5. **Azure AI Search**:  
Uses vectors produced by the embedding model to search for relevant and semantically similar documents from the database.
   
6. **Cosmos DB**:  
The database containing catalogues, product information, and customer data, which is queried and used to generate responses.

7. **Chat Completion Model**:  
Combines vectorized prompts from the embedding model with knowledge from Azure AI Search to generate a chat response. This response is sent back to the user via API.

8. **Text to Speech Model**:  
Converts the chat response produced into an audio output using models like ElevenLabs.

9. **Evaluation Model**:  
Benchmarks the performance of the chat completion model by systematically testing it through detailed metrics.


## Interaction Flow

![Our Interaction Flow](https://microsoft-contoso-group-project.github.io/website/img/inter_flow.png)


1. **User Prompt**:  
The user provides a prompt via the chat interface.
2. **Transcription (if needed)**:  
Audio prompts are transcribed into text using the Whisper model.
3. **Query Handling**:  
The text prompt is processed by the chat function and sent to the embedding model.
4. **Semantic Search**:  
The embedding model converts the query into vectors, which are then used by Azure AI Search to find relevant documents in Cosmos DB.
5. **Response Generation**:  
The chat completion model combines information from the embedding model and Azure AI Search to generate a response.
6. **Output Delivery**:  
The response is sent back to the user. If the user prefers audio, it is converted using a text to speech model.

This architecture ensures a seamless and efficient flow of information, providing users with accurate and contextually relevant responses.
