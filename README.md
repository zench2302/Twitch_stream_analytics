# 📌 Twitch Topic Extraction & Sentiment Analysis

This project builds a real-time system to extract dominant topics and sentiment streams from Twitch chat logs. Designed to detect mood shifts and evolving discussions in live gaming streams, it combines NLP, clustering, and visualization techniques to reveal hidden structures in noisy user-generated text.

## 🔧 Key Technologies

- **BERTopic + UMAP + HDBSCAN** for topic modeling  
- **VADER + GPT-based** sentiment refinement  
- **WebSocket-based** real-time data ingestion  
- **Tokenized message segmentation** with time slicing

## 🌟 Highlights

- Handled 10K+ chat lines per minute  
- Visualized evolving topic clusters across time  
- Used **GPT-4** to refine topic summaries and labels  
- Applied to high-audience gaming streams with no user ID access

## 📈 Pipeline Overview

<img width="500" height="450" alt="image" src="https://github.com/user-attachments/assets/13bd3e65-47ea-4905-bba9-c72e2d951799" />



```
1. Real-time chat log collection via Twitch API
2. Text preprocessing and tokenization
3. Topic modeling using BERTopic
4. Sentiment analysis (VADER baseline + GPT refinement)
5. Temporal segmentation for dynamics
6. Visualization of topic shifts across streams
```

## Key Visuals
### EDA
**Message count heatmap of Games and Channels**
<img width="880" height="640" alt="image" src="https://github.com/user-attachments/assets/727002dd-8d3f-4edf-8fa5-57cf4e7afa32" />

### Sentiment Analysis 

<img width="1666" height="982" alt="image" src="https://github.com/user-attachments/assets/ba0f0303-9beb-4bd1-b357-b8c29ddcd9ac" />

### Text Clustering
<img width="1440" height="944" alt="image" src="https://github.com/user-attachments/assets/cc7b4de6-1353-4b81-a676-bbf0003646d4" />
