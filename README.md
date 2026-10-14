📩 SMS Spam Detection Using Deep Learning (LSTM)

A deep learning project that automatically classifies SMS messages as Spam or Ham (Legitimate) using an LSTM neural network built with TensorFlow and Keras.

🚀 Project Overview

Spam messages can contain unwanted advertisements, misleading offers, and suspicious links. This project uses Natural Language Processing (NLP) and deep learning to identify potentially unwanted SMS messages.

The model learns patterns from labelled messages and predicts whether a new SMS is spam or legitimate.

🎯 Objectives

- Clean and preprocess SMS text data.
- Convert text into numerical sequences using tokenization and padding.
- Build and train an LSTM classification model.
- Evaluate the model using standard classification metrics.
- Test the trained model on unseen SMS messages.

📊 Dataset

Source: "SMS Spam Detection Dataset — Kaggle" (https://www.kaggle.com/datasets/vishakhdapat/sms-spam-detection-dataset)

- Uses up to 2,000 labelled messages.
- Ham (0): Legitimate SMS.
- Spam (1): Unwanted or suspicious SMS.

🛠️ Tech Stack

- Python
- Google Colab
- TensorFlow / Keras
- Pandas and NumPy
- Scikit-learn
- Matplotlib

🧠 Model Architecture

The project uses an LSTM (Long Short-Term Memory) neural network.

SMS Message
     ↓
Text Preprocessing
     ↓
Tokenization
     ↓
Sequence Padding
     ↓
Embedding Layer
     ↓
LSTM Layer
     ↓
Dropout
     ↓
Dense Layer
     ↓
Sigmoid Output
     ↓
Spam or Ham Prediction

Why LSTM?

LSTM is designed to learn patterns and dependencies in sequential data. This makes it a suitable model to experiment with when classifying text messages.

⚙️ Project Workflow

1. Load the labelled SMS dataset.
2. Handle missing values and duplicate messages.
3. Clean the message text.
4. Split the dataset into training, validation, and testing sets.
5. Tokenize messages and pad sequences.
6. Train the LSTM model.
7. Evaluate performance on the held-out test set.
8. Predict labels for unseen messages.

📈 Evaluation Metrics

The model is evaluated using:

- Accuracy: Overall proportion of correct predictions.
- Precision: Proportion of predicted spam messages that are actually spam.
- Recall: Proportion of actual spam messages correctly identified.
- F1-score: Balance between precision and recall.

See "evaluation_metrics.csv" for the measured results.

📉 Visual Results

The repository includes the following evaluation visualizations:

- "confusion_matrix.png" — Correct and incorrect classifications.
- "accuracy_graph.png" — Training and validation accuracy.
- "loss_graph.png" — Training and validation loss.

🧪 Example Predictions

The notebook demonstrates predictions on unseen SMS messages, including suspicious prize offers and ordinary messages about college notes.

Predictions are model estimates, not guarantees that a message is safe or malicious.

📁 Repository Contents

File| Description
"SMS_Spam_Detection_LSTM.ipynb"| Complete Google Colab notebook
"spam_lstm.keras"| Trained LSTM model
"tokenizer.pkl"| Fitted text tokenizer
"config.json"| Model configuration
"evaluation_metrics.csv"| Test evaluation metrics
"confusion_matrix.png"| Confusion matrix
"accuracy_graph.png"| Accuracy plot
"loss_graph.png"| Loss plot

▶️ How to Run

1. Open "SMS_Spam_Detection_LSTM.ipynb".
2. Open the notebook in Google Colab.
3. Upload the dataset ZIP or CSV when prompted.
4. Run the notebook cells in order.
5. Review the training metrics, graphs, and example predictions.

🔮 Future Improvements

- Compare LSTM with Simple RNN and GRU.
- Evaluate on larger and more diverse SMS datasets.
- Tune model parameters to improve generalization.
- Build an interactive web application for SMS classification.
- Explore deployment for mobile-friendly spam screening.

👨‍💻 Author

Sanjay V.

Developed as a learning project in deep learning and Natural Language Processing (NLP).

---

⭐ If you find this project useful, consider giving the repository a star.
