# ☁️ Cloud-Based Data Analysis Pipeline (AWS)

This project demonstrates an *end-to-end cloud-based data analysis pipeline* using *AWS, Python, Pandas, Docker, and Git*. It simulates a real-world workflow where data is stored in the cloud, processed on a compute instance, and analyzed using a containerized application.

---

## 📌 Project Overview

* *Data Source*: Real-world CSV dataset (Kaggle-style sales data)
* *Storage*: AWS S3
* *Compute*: AWS EC2
* *Processing*: Python & Pandas
* *Containerization*: Docker
* *Version Control*: Git

The application reads data from S3, performs basic analytics, and outputs insights such as total sales and category-wise summaries.

---

## 🏗️ Architecture


Local Machine → GitHub
        ↓
     AWS EC2 (Dockerized Python App)
        ↓
     AWS S3 (CSV Dataset)


---

## 📂 Project Structure


cloud-sales-analytics/
│
├── data/
│   └── train.csv
│
├── scripts/
│   └── analysis.py
│
├── requirements.txt
├── Dockerfile
└── README.md


---

## 📊 Dataset

* Format: CSV
* Uploaded to: *AWS S3 Bucket*
* Example columns:

  * Order ID
  * Category
  * Sales
  * Profit

---

## 🛠️ Technologies Used

* *Python 3.10*
* *Pandas* – data analysis
* *AWS S3* – object storage
* *AWS EC2* – compute instance
* *Docker* – containerization
* *Git* – version control

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

bash
git clone <your-repo-url>
cd cloud-sales-analytics


---

### 2️⃣ Install Dependencies (Local Test)

bash
pip install -r requirements.txt
python scripts/analysis.py


---

### 3️⃣ Build Docker Image

bash
docker build -t cloud-sales-analytics .


---

### 4️⃣ Run Docker Container

bash
docker run cloud-sales-analytics


---

## ☁️ AWS Deployment Steps (High Level)

1. Create an *S3 bucket* and upload train.csv
2. Launch an *EC2 instance*
3. Install Docker on EC2
4. Pull project code from GitHub
5. Build & run Docker container on EC2

---

## 📈 Sample Output

* Total Sales
* Category-wise Sales Summary
* Basic statistical insights

---

## 🎯 Learning Outcomes

* Hands-on experience with AWS S3 and EC2
* Practical data analysis using Pandas
* Understanding Docker-based deployment
* Real-world cloud data pipeline exposure

---

## 🚀 Future Enhancements

* Add data visualization (Matplotlib / Seaborn)
* Automate pipeline using cron jobs
* Integrate Streamlit dashboard
* Add IAM roles for secure S3 access

---

## 👩‍💻 Author

*Dhanashree Pogade*
Aspiring Data Analyst | Cloud & Python Enthusiast
