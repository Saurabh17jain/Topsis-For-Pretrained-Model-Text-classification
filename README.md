# TOPSIS-Based Model Selection for Text Classification

## 📌 Overview

This project implements the **TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution)** method to rank different text classification models based on multiple performance criteria. The models are evaluated on accuracy, F1-score, inference time, and model size, helping to select the best trade-off between performance and efficiency.

## 🚀 Features

- **Multi-Criteria Decision Making**: Considers multiple metrics to rank models.
- **Customizable Weights & Impacts**: Adjust importance for accuracy, F1-score, inference time, and size.
- **Correct TOPSIS Implementation**: Uses vector normalization for accurate ranking.
- **Easy-to-Use Python Code**: Works with any dataset containing model evaluation metrics.
- **Graphical Representation**: Generates visual insights with tables and plots.

## 📂 Dataset

The dataset consists of evaluation metrics for different NLP models:

| Model      | Accuracy | F1-score | Inference Time (ms) | Model Size (MB) |
| ---------- | -------- | -------- | ------------------- | --------------- |
| BERT       | 0.89     | 0.88     | 12                  | 420             |
| RoBERTa    | 0.91     | 0.92     | 14                  | 500             |
| DistilBERT | 0.87     | 0.86     | 8                   | 250             |
| XLNet      | 0.90     | 0.91     | 20                  | 700             |
| ALBERT     | 0.88     | 0.87     | 10                  | 200             |

## 🔧 Installation

Ensure you have Python installed, then install dependencies:

```bash
pip install numpy pandas matplotlib seaborn
```

## 🛠 Usage

Run the Python script to rank models based on TOPSIS:

```bash
python topsis_model_selection.py
```

### Example Code:

```python
ig
```

## 📊 Expected Output

The models will be ranked based on their **TOPSIS Score**, and a bar chart will be generated:

| Rank | Model      | TOPSIS Score |
| ---- | ---------- | ------------ |
| 1    | RoBERTa    | 0.79         |
| 2    | XLNet      | 0.72         |
| 3    | BERT       | 0.67         |
| 4    | ALBERT     | 0.62         |
| 5    | DistilBERT | 0.58         |

### **Graph Output:**

A bar chart will display the **TOPSIS Scores** for each model, providing a clear visual representation of their rankings.

## 🎯 Customization

- Modify the `weights` list to prioritize different metrics.
- Adjust the `impacts` array (`'+'` for maximization, `'-'` for minimization).
- Use your dataset by replacing the example values in `data`.



## 🤝 Contributing

Feel free to submit issues and pull requests! 🚀

