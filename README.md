# capstone_project_danantara_sentiment_analysis
Sentiment analysis of public opinion on Danantara using IBM Granite and Python.
# Danantara Sentiment Analysis

Analisis sentimen publik terhadap rencana pendirian **Danantara** menggunakan dataset Twitter/X, IBM Granite LLM, dan Python.  
Proyek ini merupakan bagian dari **Capstone Project** untuk memanfaatkan teknik NLP (Natural Language Processing) dalam menganalisis persepsi masyarakat terhadap isu strategis nasional.

---

## Tujuan
- Mengklasifikasikan sentimen masyarakat Indonesia terkait Danantara ke dalam kategori **positif, negatif, netral**.  
- Mengidentifikasi **common words** dominan pada tiap label sentimen.  
- Mengevaluasi indikasi penggunaan **buzzer** dalam komunikasi publik pemerintah.  
- Memberikan **rekomendasi kebijakan** berdasarkan hasil analisis.

---

## Dataset
https://docs.google.com/spreadsheets/d/12hopTaotyYxsiaZUAFNMJJ4TPtmI-U8k/edit?usp=sharing&ouid=105021870015372986372&rtpof=true&sd=true
- **Sumber**: Twitter/X  
- **Jumlah Data**: 4.639 tweet  
- **Periode**: [20-28 Februari 2025]  
- **Label**: Positif, Negatif, Netral  

---

## ⚙️ Tools & Libraries
- **Bahasa Pemrograman**: Python (Google Colab)  
- **Model**: IBM Granite LLM (via Replicate API)  
- **Libraries**:  
  - Data Processing: `pandas`, `numpy`  
  - NLP: `sastrawi`, `nltk`, `re`  
  - Visualization: `matplotlib`, `seaborn`, `plotly`, `squarify`, `wordcloud`  
  - Export: `openpyxl`, `python-docx`

---

## 📈 Hasil Utama
- **Distribusi Sentimen**:  
  - 40.3% Positif  
  - 30.0% Negatif  
  - 29.7% Netral  

- **Temuan**:  
  - Sentimen positif didominasi oleh **hashtag** seperti `#danantaraporosinvestasi` dan `#danantarabangunnegeri` (26.5% dari total tweet).  
  - Hal ini menimbulkan indikasi adanya **buzzer** yang digunakan untuk menciptakan kesan positif.  
  - Sentimen negatif didominasi oleh isu **korupsi, beban APBN, dan ketidakpercayaan pada SDM pengelola**.

---

## 💡 Rekomendasi
- **Transparansi**: Pemerintah perlu membuka mekanisme pengelolaan Danantara secara jelas dan terukur.  
- **Komunikasi Publik**: Kurangi ketergantungan pada buzzer, perbanyak komunikasi berbasis data dan fakta.  
- **Kebijakan**: Fokus pada regulasi tata kelola dana dan pengawasan independen.  

---
