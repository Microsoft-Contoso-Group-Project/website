# 1| Evaluation

A thorough evaluation process is conducted for ChatGPT models as well as a number of free Hugging Face models to assess their performance in generating text responses. The detailed methodology and results of this evaluation are presented on this page.

---

## Methodology

Each of the models is evaluated based on four metrics: Coherence, Groundedness, Fluency, and Relevance. Our evaluation process involves the use of Python scripts that calculate a weighted sum score for each model and automatically select the best-fitting model.
Our evaluation system recommends the best model and model parameters based on a weighted sum score of the four evaluation metrics.

### Auto-Evaluation Process

1. **Check if Model Exists in Connection List**
2. **Update Vector Search Based on Embedding**
3. **Calculate the 4 Evaluation Metrics**
4. **Save Results and Update Log Files**
5. **Create Summary Table**
6. **Populate HTML Page and Save to Local Directory**

The system returns a dynamic HTML page that the developer can interact with to view results.

## Results

- **Paid vs. Free Models**:  
Free models do not perform as well as the paid ChatGPT 3.5, which scores high in each of the four metrics. However, each free model has its own strength (e.g., groundedness for meta_llama3 and fluency for phi_3).
- **Flexibility**:  
Companies can easily switch between different free models based on the features they prioritize.

### Model Performance Comparison

Below are the spider graphs representing the evaluation metrics for the top models:

#### Graph 1: Top 4 Models Evaluation Results

<img src="https://microsoft-contoso-group-project.github.io/website/img/top4.svg" alt="Spider Graph 3" width="500" height="300">

#### Graph 2: Model meta_llama3_instruct_70B with different model configurations

<img src="https://microsoft-contoso-group-project.github.io/website/img/meta_llama.svg" alt="Spider Graph 3" width="500" height="300">

#### Graph 3: Model Phi_3_mini_4k_instruct with different model configurations

<img src="https://microsoft-contoso-group-project.github.io/website/img/phi3.svg" alt="Spider Graph 3" width="500" height="300">

