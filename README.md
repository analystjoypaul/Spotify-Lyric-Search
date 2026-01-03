# Spotify Lyric Search Engine  
**BM25-powered Information Retrieval System**

🔗 **Live Demo:** [spotify lyrics search](https://spotify-lyrics.streamlit.app/) 

##  Overview

The **Spotify Lyric Search Engine** is a **production-ready information retrieval application** that identifies the **exact song title and artist** from a short snippet of lyrics.

Unlike recommendation systems that suggest similar songs, this project solves a **text identification problem** using **BM25 (Okapi)** — a proven, industry-standard ranking algorithm used in search engines.


##  Key Features

 Exact song & artist identification from lyric snippets  
-  BM25 (Okapi) ranking for high-precision text search  
-  Robust text preprocessing using NLTK  
-  Built-in model evaluation (Top-1 & Top-3 Accuracy)  
-  Cached model loading for fast response time  
-  Clean, interactive Streamlit web interface  
-  Scales efficiently to 50,000+ songs  


## Why BM25?

BM25 is a **probabilistic information retrieval algorithm** widely used in:
- Search engines
- Document retrieval systems
- Enterprise search platforms

| Method | Suitability for Lyric Snippets |
|------|--------------------------------|
| TF-IDF | Medium |
| Word Embeddings | Overkill |
| **BM25** | ✅ Best Choice |

BM25 excels at **short, sparse queries**, making it ideal for lyric-based search.


##  Tech Stack

- **Python 3.9+**
- **Streamlit** – Web UI
- **Pandas** – Data processing
- **NLTK** – Text preprocessing
- **rank-bm25** – BM25 retrieval engine

##  System Architecture

1. Lyrics are cleaned and tokenized  
2. BM25 indexes the entire lyrics corpus  
3. User submits a short lyric snippet  
4. BM25 ranks songs by relevance  
5. Top-K matches are returned with confidence scores  


## Project Screenshots

![Home Page](https://github.com/analystjoypaul/Spotify-Lyric-Search/blob/master/live-demo.png)



### Clone the Repository
```bash
git clone https://github.com/<analystjoypaul>/spotify-lyric-search.git
cd spotify-lyric-search


