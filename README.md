# End-to-End Student Performance Prediction

## 📋 Project Summary

This project is an end-to-end machine learning pipeline for predicting student performance based on demographic and academic features. It includes data ingestion, preprocessing, model training, evaluation, and a Flask web interface for making predictions.

## 🛠️ Tech Stack

- Python 3.11
- Pandas, NumPy
- scikit-learn
- XGBoost, CatBoost
- Flask
- Jupyter Notebook
- Docker (optional)
- Homebrew (for Mac dependencies)
- Logging & Exception Handling

## 🚀 How to Run

### 1. Clone the Repository

```sh
git clone https://github.com/yourusername/mlproject-main.git
cd mlproject-main
```

### 2. Set Up Virtual Environment

```sh
python3 -m venv mlenv
source mlenv/bin/activate
```

### 3. Install Dependencies

```sh
pip install -r requirements.txt
```

> **Mac Users:**  
> If using XGBoost, install OpenMP:
> ```sh
> brew install libomp
> export LDFLAGS="-L/opt/homebrew/opt/libomp/lib"
> export CPPFLAGS="-I/opt/homebrew/opt/libomp/include"
> ```

### 4. Prepare Data

Place your dataset at `notebook/data/stud.csv`.

### 5. Run the Pipeline

```sh
python3 -m src.components.data_ingestion
```

### 6. Start the Flask App

```sh
python3 app.py
```

Visit [http://localhost:5001](http://localhost:5001) in your browser.

## 📁 Project Structure

```
mlproject-main/
├── app.py
├── src/
│   ├── components/
│   ├── pipeline/
│   ├── utils.py
│   ├── exception.py
│   └── logger.py
├── artifacts/
├── notebook/
│   └── data/
├── requirements.txt
└── README.md
```

## ✨ Features

- Data ingestion and preprocessing
- Multiple regression models with hyperparameter tuning
- Model evaluation and selection
- Web interface for predictions

## 📧 Contact

For questions, open an issue or contact [siddheshshanmugam@outlook.com](mailto:siddheshshanmugam@outlook.com).