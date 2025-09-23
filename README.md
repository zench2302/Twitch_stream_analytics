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

<img width="1660" height="898" alt="image" src="https://github.com/user-attachments/assets/29eca0b9-2178-4428-bcf6-64e2010a1fbb" />


### Text Clustering
<img width="1434" height="846" alt="image" src="https://github.com/user-attachments/assets/ec192bfa-4aa8-4133-8c33-74f72eb0612e" />

This one is in fact a 3D interactive scatter plot, here is just a screenshot. 
Dig into more here if interested: 


