**Task 1: News Topic Classifier Using BERT**

**Objective**

The objective of this project is to fine-tune a pre-trained BERT (Bidirectional Encoder Representations from Transformers) model to classify news headlines into four distinct categories: World, Sports, Business, and Sci/Tech. This task demonstrates the application of state-of-the-art NLP techniques for automated content categorization using the AG News Dataset.


**Methodology / Approach**

To fulfill the task requirements, the following systematic approach was implemented:

**. Data Preprocessing:** The AG News dataset was loaded and tokenized using the BertTokenizer from the bert-base-uncased checkpoint. Sequences were padded and truncated to a maximum length of 128 tokens for optimal performance.

**. Model Training:** I fine-tuned the BertForSequenceClassification model using the Hugging Face Trainer API. The training was conducted for 3 epochs with a learning rate of 2e-5 and a weight decay of 0.01.

**. Evaluation:** The model's performance was monitored at each epoch using Accuracy and Weighted F1-score to ensure robust classification across all four classes.

**. Deployment:** A live, interactive web interface was developed using Gradio, allowing users to input headlines and receive real-time topic predictions.


**Key Results & Observations**

The model achieved high performance, significantly exceeding the standard requirements for text classification:

**Final Accuracy: ~94.7%.**

**Weighted F1-Score: ~0.947.**

**Observations: The model demonstrates exceptional precision in distinguishing between "Sports" and "World" news. A minor overlap exists between "Business" and "Sci/Tech," which is consistent with real-world news where technology and business sectors frequently intersect.**


**Technologies Used**

**.Python**

**.Hugging Face Transformers & Datasets**

**.PyTorch**

**.Gradio (for deployment)**

**.Scikit-learn (for evaluation metrics)** 
