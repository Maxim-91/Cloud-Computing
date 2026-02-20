# Module 1: a basic ML model using Google Teachable Machine
The model was created using Google Teachable Machine, an AutoML tool that simplifies the ML process by automating manual steps. It is trained to recognize six specific classes: Glass, Cup, Table, Chair, Sofa, and Candle.

### Project Structure: `my_model`
The `my_model` folder contains the exported **TensorFlow.js** files necessary for the application to function:
* `model.json`: The model architecture.
* `weights.bin`: The learned parameters (weights).
* `metadata.json`: Information about the 6 object classes (Glass, Cup, Table, Chair, Sofa, and Candle).

### How to Use

1.  **Placement**: Ensure the `index.html` file and the `my_model` folder (containing the three files above) are in the same directory.
2.  **Run a Server**: To function correctly, the application must be opened via a web server. 
    * **Recommended**: In Visual Studio Code, right-click `index.html` and select **"Open with Live Server"**.
3.  **Interaction**: 
    * Click the **"Launch Camera"** button.
    * The model will scan the video frame for objects.
    * When an item is detected (e.g., a **Chair** or **Candle**), its name will highlight in **green** on the UI list.

---
# Module 2: NLP in Cloud Enviroment
This project focuses on Natural Language Processing (NLP) in cloud environments, specifically performing sentiment analysis on a textual dataset using classical machine learning techniques.
The model to classify text reviews into three categories: **positive**, **neutral**, and **negative**. The project was developed in a cloud-based environment using **Google Colab**.

### Tech Stack
* **Platform**: Google Colab.
* **Libraries**: Pandas, Scikit-learn (LinearSVC), NumPy.
* **Methodology**: TF-IDF (Term Frequency-Inverse Document Frequency) vectorization.
* **Dataset**: [Sentiment Analysis Dataset (Kaggle)](https://www.kaggle.com/datasets/abhi8923shriv/sentiment-analysis-dataset) — specifically the `test.csv` (474.04 kB) file.

### Key Implementation Steps
1.  **Data Cleaning**: Removed nearly 1,300 missing values to ensure the reliability of the training process.
2.  **Data Split**: The dataset was divided into training (70%) and testing (30%) sets.
3.  **Pipeline Construction**: Built a systematic pipeline that converts raw text into numerical vectors using TF-IDF and passes them to a **Linear Support Vector Classifier (LinearSVC)**.
4.  **Evaluation**: Utilized diverse metrics, including a **Classification Report** and a **Confusion Matrix**, to analyze the model's strengths and weaknesses.

### Results and Insights
* **Accuracy**: The model achieved an overall accuracy of 64%.
* **Performance**: The model is most effective at identifying "positive" sentiments (F1-score of 0.71).
* **Observation**: Manual testing showed that while the model excels at identifying explicit emotional cues (e.g., "happy", "hate"), it can struggle with subtle context or ambiguous phrasing.



