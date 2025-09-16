README.md
# 🔑 Password Strength Checker

This project uses **Machine Learning** to classify passwords as **Weak**, **Medium**, or **Strong** based on their character composition.  
It utilizes **TF-IDF Vectorization** to convert passwords into numerical features and trains a **Random Forest Classifier** to predict their strength.

---

## 📌 Features
- Classifies passwords into `Weak`, `Medium`, and `Strong` categories
- Uses **character-level TF-IDF** for password feature extraction
- Trains a **Random Forest Classifier** for high accuracy predictions
- Interactive input to check password strength manually

---

## 📊 Dataset
Dataset used: **Password Strength Dataset**  
📥 Download here: [Password Strength Dataset (Kaggle)](https://www.kaggle.com/datasets/bhavikbb/password-strength-classifier-dataset)  

Place the dataset in your working directory as `data.csv`.

---

## 🛠️ Installation & Usage

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/password-strength-checker.git
cd password-strength-checker

2️⃣ Install Dependencies
pip install pandas numpy scikit-learn

3️⃣ Run the Script
python password_strength_checker.py

4️⃣ Check Your Password Strength

When prompted, enter any password (input is hidden for security) and see if it is Weak, Medium, or Strong.

📈 Model Training

Preprocessing: Dropped missing values, mapped labels (0 → Weak, 1 → Medium, 2 → Strong)

Feature Extraction: TfidfVectorizer with custom character-level tokenizer

Model: RandomForestClassifier from sklearn.ensemble

Evaluation: Accuracy score displayed after training

🖼 Example
Enter Password: ********
Predicted Strength: Strong

🔮 Future Improvements

Add a web interface using Flask or Streamlit for easy access

Incorporate rules like length, presence of special characters, and numbers

Provide suggestions for improving password strength

🤝 Contributing

Pull requests and suggestions are welcome!
For significant changes, open an issue first to discuss your ideas.

📜 License

This project is licensed under the MIT License.
