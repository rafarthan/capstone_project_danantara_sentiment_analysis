# capstone_project_danantara_sentiment_analysis
Sentiment analysis of public opinion on Danantara using IBM Granite and Python.
# Danantara Sentiment Analysis

Analisis sentimen publik terhadap rencana pendirian **Danantara** menggunakan dataset Twitter/X, IBM Granite LLM, dan Python.  
Proyek ini merupakan bagian dari **Capstone Project** untuk memanfaatkan teknik NLP (Natural Language Processing) dalam menganalisis persepsi masyarakat terhadap isu strategis nasional.

## Tujuan
- Mengklasifikasikan sentimen masyarakat Indonesia terkait Danantara ke dalam kategori **positif, negatif, netral**.  
- Mengidentifikasi **common words** dominan pada tiap label sentimen.  
- Mengevaluasi indikasi penggunaan **buzzer** dalam komunikasi publik pemerintah.  
- Memberikan **rekomendasi kebijakan** berdasarkan hasil analisis.

## Dataset
https://docs.google.com/spreadsheets/d/12hopTaotyYxsiaZUAFNMJJ4TPtmI-U8k/edit?usp=sharing&ouid=105021870015372986372&rtpof=true&sd=true
- **Sumber**: Twitter/X  
- **Jumlah Data**: 4.639 tweet  
- **Periode**: [20-28 Februari 2025]  
- **Label**: Positif, Negatif, Netral  

## Tools & Libraries
- **Bahasa Pemrograman**: Python (Google Colab)  
- **Model**: IBM Granite LLM (via Replicate API)  
- **Libraries**:  
  - Data Processing: `pandas`, `numpy`  
  - NLP: `sastrawi`, `nltk`, `re`  
  - Visualization: `matplotlib`, `seaborn`, `plotly`, `squarify`, `wordcloud`  
  - Export: `openpyxl`, `python-docx`

## AI Explanation
Proyek ini memanfaatkan **Large Language Model (LLM) IBM Granite** untuk melakukan **klasifikasi sentimen otomatis** pada data tweet.  
Berikut penjelasan perannya dalam pipeline:

1. **Mengapa AI Digunakan?**
   - Jumlah data (ribuan tweet) terlalu besar untuk dilabeli manual.
   - LLM mampu memahami konteks bahasa Indonesia dengan baik, termasuk sarkasme dan frasa tidak formal.
   - Memberikan hasil yang lebih **scalable dan efisien** dibanding metode manual.

2. **Bagaimana Cara Kerjanya?**
   - Data tweet mentah diproses melalui tahapan **preprocessing**.
   - IBM Granite LLM menerima prompt **instruksi klasifikasi** (positif, negatif, netral).
   - Model mengembalikan output label untuk tiap tweet dengan format terstandarisasi.
   - Hasil prediksi dipadukan dengan dataset berlabel untuk **analisis lanjutan**.

3. **Kontribusi AI dalam Project**
   - **Automatisasi Labeling**: Mempercepat klasifikasi ribuan tweet yang sebelumnya tidak berlabel.
   - **Consistency**: Memberikan label dengan aturan seragam sesuai definisi sentimen yang ditentukan.
   - **Insight Discovery**: Membantu menemukan pola kata/kalimat dominan yang memengaruhi klasifikasi.
   - **Decision Support**: Hasil analisis sentimen dipakai untuk menyusun **rekomendasi kebijakan publik** terkait Danantara.
Dengan AI, proyek ini berhasil mengubah data mentah dari Twitter menjadi **informasi strategis** yang relevan untuk pemerintah maupun peneliti.

## Hasil Utama
- **Distribusi Sentimen**:  
  - 40.3% Positif  
  - 30.0% Negatif  
  - 29.7% Netral  

- **Temuan**:  
  - Sentimen positif didominasi oleh **hashtag** seperti `#danantaraporosinvestasi` dan `#danantarabangunnegeri` (26.5% dari total tweet).  
  - Hal ini menimbulkan indikasi adanya **buzzer** yang digunakan untuk menciptakan kesan positif.  
  - Sentimen negatif didominasi oleh isu **korupsi, beban APBN, dan ketidakpercayaan pada SDM pengelola**.

## Rekomendasi
- **Transparansi**: Pemerintah perlu membuka mekanisme pengelolaan Danantara secara jelas dan terukur.  
- **Komunikasi Publik**: Kurangi ketergantungan pada buzzer, perbanyak komunikasi berbasis data dan fakta.  
- **Kebijakan**: Fokus pada regulasi tata kelola dana dan pengawasan independen.  
