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

```
1. Real-time chat log collection via Twitch API
2. Text preprocessing and tokenization
3. Topic modeling using BERTopic
4. Sentiment analysis (VADER baseline + GPT refinement)
5. Temporal segmentation for dynamics
6. Visualization of topic shifts across streams
```
