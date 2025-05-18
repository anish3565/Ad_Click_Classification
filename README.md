# 🧠 Advertisement Click Classification

## 📌 Overview

This project focuses on predicting whether a user will click on an online advertisement based on their behavioral and demographic attributes. By leveraging machine learning techniques, we aim to assist marketers in optimizing ad placements and targeting strategies.

## 📂 Dataset

The dataset comprises user information and their interaction with online advertisements. Key features include:

* **Daily Time Spent on Site**: Time (in minutes) the user spends on the website.
* **Age**: Age of the user.
* **Area Income**: Average income of the user's geographical area.
* **Daily Internet Usage**: Average time (in minutes) the user spends on the internet.
* **Ad Topic Line**: The headline of the advertisement.
* **City**: City of the user.
* **Male**: Gender indicator (1 for male, 0 for female).
* **Timestamp**: Date and time of the user’s interaction.
* **Clicked on Ad**: Target variable indicating whether the user clicked on the ad (1) or not (0).

## 🧪 Project Workflow

1. **Data Exploration & Preprocessing**:

   * Loaded and inspected the dataset for missing values and data types.
   * Performed exploratory data analysis (EDA) to understand feature distributions and relationships.
   * Converted categorical variables and timestamps into numerical formats suitable for modeling.

2. **Feature Engineering**:

   * Extracted additional features from the timestamp, such as hour and day of the week.
   * Normalized numerical features to ensure uniform scaling.

3. **Model Building**:

   * Split the dataset into training and testing sets.
   * Implemented various classification algorithms:

     * Logistic Regression
     * Decision Tree
     * Random Forest
     * AdaBoost
   * Evaluated models using metrics like accuracy, precision, recall, and F1-score.

4. **Model Evaluation & Selection**:

   * Compared model performances to select the best-performing algorithm.
   * Fine-tuned hyperparameters to optimize model accuracy.

5. **Model Deployment**:

   * Serialized the final model using `pickle` for future predictions.
   * Provided a sample script to demonstrate loading the model and making predictions on new data.

## 📊 Results

* The **AdaBoost Classifier** outperformed other models, achieving high accuracy and robustness against overfitting.
* Feature importance analysis revealed that **Daily Time Spent on Site** and **Age** were significant predictors of ad clicks.

## 🛠️ Technologies Used

* **Programming Language**: Python
* **Libraries**:

  * Data Manipulation: `pandas`, `numpy`
  * Visualization: `matplotlib`, `seaborn`
  * Machine Learning: `scikit-learn`
  * Model Serialization: `pickle`

## 🚀 Getting Started

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/anish3565/Ad_Click_Classification.git
   cd Ad_Click_Classification
   ```

2. **Install Dependencies**:
   Ensure you have Python 3.x installed. Then, install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Notebook**:
   Open and execute the Jupyter Notebook to explore the analysis and model building steps:

   ```bash
   jupyter notebook AdClickClassification.ipynb
   ```

4. **Make Predictions**:
   Use the provided script to load the serialized model and make predictions on new data.

## 📁 Project Structure

```
Ad_Click_Classification/
├── Dataset/
│   └── advertising.csv
├── AdClickClassification.ipynb
├── FinalAdaboostModel.pkl
├── requirements.txt
└── README.md
```

## 🤝 Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to fork the repository and submit a pull request.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 📬 Contact

For questions or feedback, please reach out to [anish3565](https://github.com/anish3565).
