# 2024 U.S. Election Sentiment on X 🇺🇸

Welcome to the 2024 U.S. Election Sentiment Analysis project! This project aims to analyze public sentiment and trends from the 2024 U.S. election using real-time data from X (formerly Twitter). Let's dive into the details! 🚀

## Overview

In this project, we explore the dynamics of the 2024 U.S. Presidential Race by analyzing tweets to capture public sentiment, critical policy discussions, and party-level engagement. This dataset provides a unique opportunity to analyze real-time public reactions during one of the most pivotal election years in history.

## Dataset 📊

### Title
**2024 U.S. Presidential Race on X: Sentiment and Trends**

### Description
Uncover the dynamics of the 2024 U.S. Presidential Race with this robust dataset from X, capturing public sentiment, critical policy discussions, and party-level engagement. This dataset provides an unparalleled opportunity to analyze real-time public reactions during one of the most pivotal election years in history.

### Dataset Highlights
- **Comprehensive Candidate Coverage**: Includes data on major contenders such as Kamala Harris (Democratic Party), Donald Trump (Republican Party), Jill Stein (Green Party), Chase Oliver (Libertarian Party), and Robert Kennedy (Independent).
- **Time-Sensitive Insights**: Captures key events, debates, and policy announcements from January to February 2025.
- **Rich Metadata**: Each entry includes tweet text, timestamp, user handle, sentiment labels (positive, negative, neutral), retweets, likes, and party affiliation.
- **Practical Use Cases**: Ideal for sentiment analysis, topic clustering, real-time trend detection, and understanding the role of digital platforms in shaping electoral outcomes.
- **Actionable Insights**: Explore how social media influences voter behavior, amplifies campaign messages, and reflects societal priorities during elections.

### Source
This dataset was collected from Kaggle. Credits to Kaggle: [2024 U.S. Election Sentiment on X](https://www.kaggle.com/datasets/emirhanai/2024-u-s-election-sentiment-on-x)

## Data Description 📝

The dataset contains the following columns:
- `tweet_id`: A unique identifier for each tweet.
- `user_handle`: The username or handle of the account that posted the tweet.
- `timestamp`: The date and time when the tweet was posted.
- `tweet_text`: The content of the tweet.
- `candidate`: The political candidate mentioned in the tweet.
- `party`: The political party of the mentioned candidate.
- `retweets`: The number of times the tweet was retweeted.
- `likes`: The number of likes the tweet received.
- `sentiment`: The overall sentiment of the tweet (positive, negative, or neutral).

## Approach 🛠️

### Data Cleaning
1. **Sentiment Column**: Removed leading and trailing spaces.
2. **Tokenization**: Converted tweet text into sequences of tokens.
3. **Padding**: Padded sequences to ensure uniform length.
4. **One-Hot Encoding**: Encoded sentiment labels into one-hot vectors.
5. **Normalization**: Normalized retweets and likes.

### Models Used

#### Model 1: LSTM-based Sentiment Analysis
- **Architecture**: Embedding layer, LSTM layers, Dropout layers, Dense layers.
- **Performance**: Achieved a test accuracy of 85.20%.

#### Model 2: LSTM-based Sentiment Analysis with Additional Features
- **Architecture**: Embedding layer, LSTM layers, Dropout layers, Dense layers, additional features (retweets and likes).
- **Performance**: Achieved a test accuracy of 89.29%.

#### Model 3: Bidirectional LSTM-based Sentiment Analysis
- **Architecture**: Embedding layer, Bidirectional LSTM layers, Dropout layers, Dense layers.
- **Performance**: Achieved a test accuracy of 99.60%.

### Explanation of LSTM and Bidirectional LSTM
- **LSTM (Long Short-Term Memory)**: LSTM networks are a type of recurrent neural network (RNN) capable of learning order dependence in sequence prediction problems. They are well-suited for tasks where context from previous inputs is important.
- **Bidirectional LSTM**: Bidirectional LSTMs are an extension of traditional LSTMs that improve model performance on sequence classification problems. They involve duplicating the first recurrent layer in the network so that there are two layers side by side, providing the network with both past and future context.

### Why They Worked Well
- **LSTM**: Captures temporal dependencies in the tweet text, making it effective for sentiment analysis.
- **Bidirectional LSTM**: Enhances the model's ability to capture contextual information from both directions in the tweet text, leading to improved sentiment prediction accuracy.

## Hardware Used 💻
- **CPU**: Intel i7-13650
- **GPU**: NVIDIA RTX 3070

## Conclusion 🎉

This project successfully analyzed public sentiment and trends from the 2024 U.S. election using real-time data from X. The models developed, especially the Bidirectional LSTM-based model, demonstrated strong performance in predicting tweet sentiment, leveraging both tweet text and additional features like retweets and likes. The use of advanced neural network architectures like LSTM and Bidirectional LSTM allowed us to capture the contextual information effectively, resulting in high accuracy.

Thank you for exploring this project! Feel free to reach out if you have any questions or suggestions. Happy analyzing! 😊
