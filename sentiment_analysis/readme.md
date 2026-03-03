1. **Language Detection** – Automatically detects whether the input text is English, French, or another language using Mediapipe.  
2. **Punctuation Restoration** – Corrects missing or incorrect punctuation in unpunctuated or poorly punctuated text using a deep learning model (`deepmultilingualpunctuation`).  
3. **Sentence Splitting** – Breaks the paragraph into individual sentences for more accurate analysis.  
4. **Sentiment Analysis** – Assigns each sentence a sentiment label: **positive**, **neutral**, or **negative**, and calculates confidence scores using a lightweight multilingual model.  
5. **Visualization** – Displays a pie chart showing the distribution of sentiments across all sentences.  

---

Demo App can be visited here: **[Kakoo Sentiment App](https://sent-kakoo.streamlit.app)**

The app can handle text input **either typed directly** or **uploaded as a file**.
