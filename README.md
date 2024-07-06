# Fine-Tuning-Llama-2-on-Together.ai-for-Text-Summarization
Find more details about the project here https://medium.com/@vgupta701/fine-tuning-llama-2-on-together-ai-for-text-summarization-9d26a205d5b3

### Objective
To fine-tune a large language model (LLM) for analyzing and summarizing large volumes of customer reviews, specifically for two popular Asian restaurants in Austin, Qi Austin and 1618 Asian Fusion.

### Business Objective
To leverage AI-driven insights from customer reviews to inform business decisions, enhance customer experience, and improve service quality by effectively analyzing open-ended feedback.

### Dataset Overview
The dataset includes:
- Customer reviews scraped from Yelp.com for Qi Austin and 1618 Asian Fusion.
- A manually created tuning dataset with 200 reviews formatted to capture key topics and takeaways.

### Analysis Approach
1. **Data Collection**:
   - Extracted reviews for Qi Austin and 1618 Asian Fusion, focusing on comprehensive customer experiences and opinions.

2. **Model Selection**:
   - Chose Llama-2-7B-32K-Instruct for its efficiency and suitability for summarization tasks.
   - Opted for a smaller, more efficient model due to constraints on training time and dataset size.

3. **Fine-Tuning Process**:
   - Manually created outputs in the desired format for a subset of reviews to establish a tuning dataset.
   - Set up the data in the required prompt sequence for the model.

4. **Training Parameters**:
   - Trained the model with 8 epochs, a batch size of 1, and a learning rate of 5e-5.
   - Adjusted parameters after initial trials to improve results.

5. **Post-Processing**:
   - Extracted topics and takeaways from the model-generated output.
   - Organized takeaways for each topic into separate columns and created a detailed data frame for food items.

### Insights
1. **Model Performance**:
   - The tuned model significantly improved accuracy and formatting of summaries compared to the base model.
   - Effective extraction of key topics such as Food, Service, Ambiance, Price, and others.

2. **Customer Preferences**:
   - Identified popular food items: Fried rice at 1618 Asian Fusion and soup dumplings at Qi Austin.
   - Highlighted differences in customer feedback, such as constructive criticism for soup dumplings at 1618 Asian Fusion, suggesting areas for improvement.

3. **Price Feedback**:
   - Customers across both restaurants mentioned high prices, with stronger sentiment for Qi Austin.

### Recommendations
1. **Increase Dataset Size**:
   - Expand the tuning dataset to improve model performance and robustness.

2. **Enhance Dataset Quality**:
   - Ensure high-quality, representative samples in the tuning dataset for better model generalization.

3. **Refine Prompts and Instructions**:
   - Experiment with different system prompts and instructions to optimize the model’s summarization capabilities.

4. **Use Larger Base Models**:
   - Consider using a larger base model if computational resources allow, to potentially achieve better performance.

5. **Increase Training Epochs**:
   - Further increase training epochs to improve the model’s ability to learn from the data.

### Future Scope for Improvement
- **Incorporate Additional Data Sources**: Integrate reviews from other platforms and additional customer feedback mechanisms.
- **Explore Different Model Architectures**: Test various neural network architectures to find the most effective one for summarization.
- **Evaluate Real-Time Applications**: Develop real-time feedback systems that can provide immediate insights to businesses based on ongoing customer reviews.

