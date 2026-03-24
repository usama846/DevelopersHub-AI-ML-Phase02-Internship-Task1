Task 1: News Topic Classifier Using BERT
📝 Objective
The primary goal of this task is to fine-tune a state-of-the-art Transformer model to accurately classify news headlines into four distinct categories: World, Sports, Business, and Sci/Tech. This project demonstrates the application of Transfer Learning in Natural Language Processing (NLP) to handle real-world text classification.
+1

🛠️ Methodology & Approach
To achieve the objectives outlined by Developers Hub Corporation, the following approach was taken:
+1


Dataset Acquisition: Utilized the AG News Dataset from Hugging Face, consisting of 120,000 training samples and 7,600 test samples.


Preprocessing: * Tokenized text using the BertTokenizer from the bert-base-uncased checkpoint.

Applied padding and truncation to a max length of 128 tokens for computational efficiency.


Model Selection: Fine-tuned the bert-base-uncased model using the Hugging Face Trainer API.

Training Configuration:

Learning Rate: 2e-5

Epochs: 3

Batch Size: 16

Weight Decay: 0.01


Evaluation: Monitored performance using Accuracy and Weighted F1-score to ensure balanced classification across all topics.
+1


Deployment: Created an interactive web interface using Gradio to allow for real-time inference on custom news headlines.
+1

📊 Key Results & Observations
The model showed strong convergence and high predictive power:

Final Accuracy: ~94.7% (on the test set).

Weighted F1-Score: ~0.947.

Insights: The model performs exceptionally well on "Sports" and "World" categories. There is a slight, expected overlap between "Business" and "Sci/Tech" due to the shared vocabulary in technical-business reporting.
