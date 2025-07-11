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

---

## 🗂 Project Notes & Logs (Archive)

> The following are earlier notes, brainstorming, task assignments, and development logs.

### # Outline

- spam detection - user  
- specific streams  
- sentiment metric  
- gaming streamer  
- no userid  
- twitch API documentation

### # For Twitch API  
Check notebook `ST445_GAMING.ipynb`

### # For Data Collection and Writing to BigQuery  
Check notebook `twitch_chat_liste.ipynb`

**1. Game List**  
Now the game list is selected manually from [Twitch Gaming Directory](https://www.twitch.tv/directory/gaming), using recommended games and popular ones.  
> ⚠️ Considered scraping, but API limits make it challenging.

**2. Channel List**  
Selected top 20 channels per game by real-time viewer count. Focused on frequent group activity as a proxy for emergent community behavior.

---

### 📅 7 May Meeting Log

**Summary:**

1. **Data acquisition** (by @Zench2302)  
   ✅ Done. Uploaded to GitHub.  
   Also shared via Drive:  
   - [twitch_chat_log20250511.csv](https://drive.google.com/file/d/1s46OOqRK9OPmBSEhHR8oSzeI_HCMedTN/view?usp=drive_link)  
   - [twitch_chat_log20250509.csv](https://drive.google.com/file/d/1s46OOqRK9OPmBSEhHR8oSzeI_HCMedTN/view?usp=drive_link)

2. **EDA**: in progress (@all)  
3. **Text modeling**  
   - 3.1 Tokenization: @jia & @shameek  
   - 3.2 Community detection: @shameek  
   - 3.3 Graph quant modeling: @shameek  

📍**Next meeting**: 14 May
