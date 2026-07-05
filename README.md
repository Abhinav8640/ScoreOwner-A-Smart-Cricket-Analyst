# 🏏 Cricket Player Performance Predictor

A machine learning project built with **Python** and **Scikit-learn** that predicts a cricket player's batting performance based on historical match data.

The model estimates a player's expected performance against a specific opponent at a particular venue and match format by using a **Linear Regression** model trained on past records.

---

## 📌 Features

- Predicts batting performance using historical match data.
- Uses machine learning for performance estimation.
- Supports different players, opponents, venues, and match formats.
- Calculates important batting statistics such as:
  - Predicted Runs
  - Balls Faced
  - Number of Fours
  - Number of Sixes
  - Strike Rate
  - Boundary Rate
- Handles unseen categorical values using One-Hot Encoding.
- Simple command-line interface for user interaction.

---

## 🛠️ Technologies Used

- Python
- Pandas
- Scikit-learn
- Linear Regression
- One-Hot Encoding

---

## 📂 Dataset

The dataset should contain the following columns:

| Column Name |
|-------------|
| PLAYER_NAME |
| OPPONENT_TEAM |
| VENUE |
| MATCH_FORMAT |
| RUNS_SCORED |
| BALLS_FACED |
| FOURS |
| SIXES |

Optional columns like `MATCH_ID` and `Unnamed: 0` are automatically removed if present.

---

## 🚀 How It Works

1. Load the cricket dataset.
2. Remove unnecessary columns.
3. Convert categorical columns into numerical values using One-Hot Encoding.
4. Train a Linear Regression model.
5. Take user input:
   - Player Name
   - Opponent Team
   - Venue
   - Match Format
6. Predict:
   - Runs
   - Balls Faced
   - Fours
   - Sixes
7. Calculate:
   - Strike Rate
   - Boundary Rate
8. Display the predicted batting performance.

---

## 📊 Example Output

```
Enter Player: VIRAT KOHLI
Enter Opponent Team: AUSTRALIA
Enter Venue: MUMBAI
Enter Format (only TEST/ODI): ODI

Player name:- VIRAT KOHLI
Opponent Team:- AUSTRALIA
Match Venue:- MUMBAI
Match Format:- ODI

Predicted Performance
----------------------
Runs:- 87
Balls:- 76
Aggressive Playing ⚡🔥
Fours:- 8
Sixes:- 2
Strike Rate:- 114.47
Boundary per ball:- 0.132
```

---

## 📁 Project Structure

```
Cricket-Performance-Predictor/
│
├── DATASET.csv
├── predictor.py
├── README.md
└── requirements.txt
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/cricket-performance-predictor.git
```

Navigate to the project folder:

```bash
cd cricket-performance-predictor
```

Install the required libraries:

```bash
pip install pandas scikit-learn
```

Run the project:

```bash
python predictor.py
```

---

## 📈 Machine Learning Model

- **Algorithm:** Linear Regression
- **Feature Encoding:** One-Hot Encoder
- **Train-Test Split:** 80% Training / 20% Testing
- **Multi-Output Regression:** Predicts multiple batting statistics simultaneously.

---

## 🔮 Future Improvements

- Support T20 matches.
- Predict batting average and dismissal probability.
- Add bowler-wise predictions.
- Build a graphical user interface (GUI).
- Deploy as a web application using Flask or Streamlit.
- Improve prediction accuracy using ensemble models like Random Forest or XGBoost.

---

## 🤝 Contributing

Contributions are welcome. Feel free to fork this repository, improve the project, and submit a pull request.

---

## 📄 License

This project is developed for educational and learning purposes.

---

⭐ If you found this project useful, consider giving it a star on GitHub!
