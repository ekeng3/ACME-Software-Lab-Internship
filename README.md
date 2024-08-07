# ACME-Software-Lab-Internship
# Genre Classification using Acoustic Features and Lyrics

## Introduction
This project aims to classify songs into different genres based on their acoustic features and lyrics. By leveraging machine learning and deep learning techniques, the project seeks to develop a robust model that can accurately predict the genre of a given song. Integrating acoustic and textual data is expected to improve classification performance by capturing the nuances of music that are often genre-specific.

## Objectives
The main objective of this project is:
1. Automatically classify songs into genres based on their acoustic features and lyrics.

## Methodology
The project employed a computational approach to automatically classify song genres based on the song's acoustic features and lyrics. The key steps in the methodology are:

1. **Data Collection and Source**: The data was collected from the MusicOSet platform, an enhanced open dataset of musical elements suitable for music data mining.

2. **Data Description**: The dataset contains two sets of features - acoustic features and song lyrics. The acoustic features include duration, key, mode, time signature, and various perceptual features. The lyrics data contains the song ID and the corresponding lyrics.

3. **Data Preprocessing**: The data was cleaned by handling missing values, removing duplicates, and ensuring the data was in a suitable format. The text data (lyrics) was preprocessed by removing section labels, numbers, punctuation, converting to lowercase, eliminating stop words, and lemmatizing the remaining words.

4. **Exploratory Data Analysis (EDA)**: EDA was performed to understand the data distributions, uncover relationships, and identify any outliers or imbalances in the data.

5. **Feature Engineering**: The numerical features were normalized using min-max scaling, and the genre feature was encoded using one-hot encoding. The lyrics data was encoded using word embeddings and sequence encoding techniques.

6. **Model Building and Training**: A deep learning model was developed, combining a branch for acoustic features and a branch for lyrics processing. The outputs of these branches were concatenated and passed through a final dense layer with a softmax activation for genre classification. The model was trained using the Adam optimizer and categorical cross-entropy loss, with early stopping to prevent overfitting.

## Results
The evaluation of the model's performance over 20 epochs showed significant improvement in both training and validation metrics. The final test set evaluation yielded a loss of 0.6424 and an accuracy of 83.75%, demonstrating the model's ability to generalize well to unseen data.

## Conclusion
This project successfully developed a deep learning model for genre classification by integrating acoustic features and lyrics. The results highlight the potential for advanced multi-modal approaches in music classification tasks, where leveraging both acoustic and textual data can significantly enhance performance.

## References
1. Oramas, S., Barbieri, F., Nieto Caballero, O., & Serra, X. (2018). Multimodal deep learning for music genre classification. Transactions of the International Society for Music Information Retrieval. 2018; 1 (1): 4-21.
2. Bahuleyan, H. (2018). Music genre classification using machine learning techniques. arXiv preprint arXiv:1804.01149.
3. Verdonck, T., Baesens, B., Óskarsdóttir, M., & vanden Broucke, S. (2021). Special issue on feature engineering editorial. Machine learning, 1-12.

## Acknowledgments
We would like to extend our deepest gratitude to ACME Software Lab for granting us this invaluable opportunity to be a part of the company as interns. This experience has significantly enhanced our knowledge and skills in the field of data science and machine learning.

$$$ \sum_{i=0}^{n} i^2 $$$
