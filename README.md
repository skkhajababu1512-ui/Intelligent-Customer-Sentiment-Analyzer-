# 💬 Sentiment Analysis Reviews Web Application

### 🔍 Analyze, Visualize, and Export Review Sentiments with Ease

This is a **Flask-based Web Application** that allows users to upload review datasets (CSV/TXT) or type reviews manually to perform **Sentiment Analysis** using **NLP (VADER & Transformers)**.  
It visualizes results using **Chart.js** and provides options to **download reports** in CSV and PDF formats.  

---

## 🚀 Project Overview

This project performs **Sentiment Analysis** on textual reviews and provides:
- ✅ Upload & Analyze reviews from CSV/TXT files  
- ✅ Automatic **Positive / Negative / Neutral** classification  
- ✅ Aspect-Based Sentiment Insights (e.g., service, quality, price)  
- ✅ Visualization through **Pie, Bar & Line Charts**  
- ✅ Dual highlighting for keywords (Positive, Negative, Aspect)  
- ✅ User Authentication (Login / Logout)  
- ✅ Export analyzed data in CSV and PDF formats  
- ✅ Interactive and modern user interface using **Bootstrap**  

---

## 🧠 Tech Stack & Tools Used

| Category | Technologies / Libraries |
|-----------|---------------------------|
| **Programming Language** | Python |
| **Framework** | Flask |
| **Database** | SQLite + SQLAlchemy ORM |
| **Authentication** | Flask-Login, JWT |
| **Frontend** | HTML, CSS, Bootstrap, JavaScript |
| **Visualization** | Chart.js |
| **NLP Libraries** | NLTK (VADER), Hugging Face Transformers |
| **Data Processing** | Pandas |
| **Server** | Flask Development Server |

---

## 📂 Folder Structure
sentiment-analysis-reviews-project/
│
├── static/ # CSS, JS, and assets
├── templates/ # HTML files (Flask Jinja2 templates)
│ ├── login.html
│ ├── register.html
│ ├── dashboard.html
│ ├── analysis.html
│ └── admin_dashboard.html
│
├── uploads/ # Uploaded CSV/TXT files
├── app.py # Main Flask backend application
├── models.py # SQLAlchemy models for User, Dataset, Review
├── sentiment_utils.py # Sentiment analysis logic (NLP)
├── requirements.txt # All dependencies
└── README.md # Project documentation (this file)


---

## 🧩 Features Explanation

### 1️⃣ **Login & Authentication**
- Users can **register and log in** using their credentials.  
- Authentication handled by **Flask-Login** and JWT tokens.  

### 2️⃣ **User Dashboard**
- Displays:
  - Total Datasets Uploaded
  - Total Reviews Analyzed
  - Overall Confidence Percentage  
- Allows users to:
  - Upload CSV/TXT datasets  
  - Enter manual reviews  
  - Start analysis  
  - View recent uploads  

### 3️⃣ **Sentiment Analysis**
- Uses **NLTK’s VADER** for polarity detection.  
- Optional integration with **Hugging Face Transformers** for deeper NLP.  
- Each review is analyzed and stored in the database with:
  - Raw Text
  - Preprocessed Text
  - Sentiment (Positive / Negative / Neutral)
  - Confidence Score  

### 4️⃣ **Aspect-Based Analysis**
- Detects key aspects like *service, quality, delivery, price, staff, etc.*  
- Shows **top positive and negative words** with their frequencies.  
- Highlights aspect-related terms within reviews.  

### 5️⃣ **Insights & Visuals**
- Interactive **Chart.js** visualizations:
  - 🥧 Pie Chart → Sentiment Distribution  
  - 📊 Bar Chart → Aspect-wise Sentiments  
  - 📈 Line Chart → Sentiment Trends Over Time  

### 6️⃣ **Dual Word Highlighting**
- Positive words → Green  
- Negative words → Red  
- Aspect words → White  
This feature visually enhances review readability.

### 7️⃣ **Export Section**
- Export all analyzed results in:
  - **CSV format** (full data)
  - **PDF format** (summary + sample reviews)

🏁 Conclusion

This project is a complete end-to-end Sentiment Analysis and Visualization System designed to simplify analyzing textual reviews and understanding user sentiments at a glance.
