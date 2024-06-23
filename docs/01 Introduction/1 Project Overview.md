# 1| Project Overview

## Motivation

Nowadays, businesses starts to make use of Generative AI for chatbot applications to enhance users' online shopping experience. However, many face three huge challenges:

- **Costs**:  
Deploying proprietary AI models, such as those from OpenAI on Azure, can be prohibitively expensive. Our tests indicate that maintaining these models can cost around $10 per day, which would quickly add up when the business scale increases. 
- **Integration**:  
Different models are required for embedding, chat completion, and evaluation. Choosing the right model combination and ensuring they work seamlessly together can be complex and time-consuming.
- **Accessibility**:  
There's a need to cater to a diverse user base, ensuring that AI-driven solutions are accessible and usable for everyone, including those who have difficulty reading or writing.

## Objective

This project aims to explore the viability of using open-source models from [Hugging Face](https://huggingface.co) to reconstruct the Contoso Chat retail copilot application originally developed by Microsoft. By integrating these models into the Contoso Chat application, we aim to address the challenges stated in the Motivation section and make AI chatbot more accessible to all online retailers. 

## Key Accomplishments

- **Hugging Face Model Integration**:  
Builds a framework for integrating the Hugging Face platform’s vast library of AI models with Contoso Chat for text embedding, chat completion and evaluation tasks.
- **Enhanced UI**:  
Introduces a new audio input/output feature to improve user accessibility.
- **Model Recommendation**:  
Evaluates and compares the performances of popular Large Language Models on the chat completion task. Makes automatic model recommendation based on evaluation scores.

Our testing shows promising results in terms of AI accuracy and user satisfaction. The documentation provides detailed insights into the development process and our learnings.

## Future Work

We plan to enhance the project with several key developments:

- **Add an Extra LLM Layer to Analyze Evaluation Results**:  
Implement an additional layer to process and interpret evaluation data, making the evaluation results more comprehensible for everyone.
- **Create a System to Recommend Suitable Model Configuration**:  
Develop a recommendation system to suggest optimal model configurations based on specific use cases and requirements.
- **Create a More Comprehensive Evaluation Method**:  
Design and implement more detailed and nuanced evaluation matrices to better assess model performance across various metrics and dimensions.
- **Explore Different Methods of Deploying the Whisper Model to Reduce Latency**:  
Investigate and implement various deployment strategies for the Whisper model to minimize response times and improve user experience.
- **Implement Multiple Language Support**:  
Extend the application to support multiple languages by using embeddings tailored to different linguistic contexts, making the tool accessible to a broader audience.

