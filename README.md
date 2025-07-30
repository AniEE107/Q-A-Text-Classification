# 🤖 Q&A Text Classification using PyTorch RNN
Welcome to a lightweight yet powerful RNN-based Question Classification system built with PyTorch! 🧠 This project demonstrates how to process, classify, and visualize natural language questions using a custom-built RNN.

# 🚀 Features
🧹 Custom Tokenizer & Vocabulary Builder

🧠 RNN-Based Sequence Model (Embedding → RNN → Linear)

📦 Custom PyTorch Dataset for QA pairs

📉 Training Loop with Accuracy Tracking

🔍 Prediction with Confidence Threshold

📊 Visualization of Class Distributions & Model Predictions

# 🖼️ Visual Highlights
📌 Category Distribution
<img src="https://github.com/AniEE107/Q-A-Text-Classification/blob/main/Categorical_dist.png" width="600"/>
📈 Confidence Score Plot (Example 1)
<img src="https://github.com/AniEE107/Q-A-Text-Classification/blob/main/Confidence_Score%20(2).png" width="600"/>
📈 Confidence Score Plot (Example 2)
<img src="https://github.com/AniEE107/Q-A-Text-Classification/blob/main/Confidence_score.png" width="600"/>
🗂️ Dataset
File: 100_Unique_QA_Dataset.csv

Format: Two columns — question and answer

Preprocessing: Lowercasing, punctuation cleaning, whitespace tokenization

# 📐 Model Architecture
text
Copy
Edit
Input Text → Embedding → RNN → Linear → Softmax → Category
Embedding: Transforms tokens into dense vectors

RNN: Processes sequential data

Linear: Maps RNN output to class scores

Softmax: Converts scores to probabilities

# 🛠️ Project Structure
css
Copy
Edit
📁 Q-A-Text-Classification
├── Q&A_using_RNN-PYTORCH.py      # Main script
├── 100_Unique_QA_Dataset.csv     # QA dataset
├── README.md                     # You are here!
🧪 Sample Prediction
python
Copy
Edit
predict(model, "What is the capital of France?")
# Output: Predicted: history (confidence: 0.87)
🎨 Visual Confidence Plot
python
Copy
Edit
visualize_prediction(model, "What is Machine?", index2label)
Renders a horizontal bar chart showing model confidence per class.

# 📊 Training Progress (Sample)
Epoch	Loss	Accuracy
1	525.07	21.5%
5	264.87	52.4%
10	78.56	89.1%

✅ Loss decreases steadily — model is learning effectively!

# 🧠 Future Enhancements
⏱ Use LSTM or GRU for better context understanding

🧬 Integrate pretrained embeddings (e.g., GloVe, FastText)

📱 Build a web UI with Streamlit or Gradio

🧪 Add validation/test split with metrics

# 👨‍💻 Author
Manish Kumar — GitHub Profile »
If you find this project helpful, please ⭐️ star the repo!

# 📎 License
This project is open-source under the MIT License.
