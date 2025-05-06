# 🚀 Sentiment Analysis Model with AWS and Streamlit/Gradio

## 🔍 What is this project about?

This project helps you **analyze the sentiment** of tweets — whether they are **Positive, Negative, or Neutral**. It uses a **machine learning model** and lets users interact with it through a **web app** made using **Streamlit** or **Gradio**.

The app is hosted on **AWS** so it can run smoothly and handle many users at once.

---

## 🌟 Main Features

* Check how people feel about a topic (entity-based sentiment).
* Simple web app to enter a tweet and see the result.
* Deployed on AWS for better performance.
* Saves user login info in a secure AWS database.

---

## 🧰 Tools Used

* **Machine Learning:** Hugging Face Transformers
* **Web App:** Streamlit or Gradio
* **Cloud:** AWS (S3, EC2, RDS, IAM)
* **Database:** PostgreSQL (Amazon RDS)
* **Language:** Python

---

## 📊 About the Data

Used a Twitter dataset that includes:

* Tweet ID
* Topic (Entity)
* Sentiment (Positive, Negative, Neutral)
* Tweet Text

---

## ⚙️ How to Set It Up

### ✅ What You Need

* Python 3.8 or higher
* AWS account
* AWS CLI setup
* Git installed

### 🪜 Steps to Follow

1. Clone the project:

   ```bash
   git clone https://github.com/your-username/sentiment-analysis-aws.git
   cd sentiment-analysis-aws
   ```

2. Install Python packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up AWS:

   * Start an EC2 instance
   * Upload your model to an S3 bucket
   * Set up a PostgreSQL database using Amazon RDS

4. Add your AWS and database info in a `.env` file

5. Run the app:

   ```bash
   streamlit run app.py
   # or
   python -m gradio app.py
   ```

---

## 📁 Folder Structure

```
sentiment-analysis-aws/
├── app.py            # Web app
├── requirements.txt  # Needed packages
├── model/            # Trained model
├── scripts/          # Helper scripts
├── data/             # Sample data
├── .env              # Your secrets (not shared)
└── README.md         # Info about the project
```

---

## 🚀 How to Deploy on AWS

1. Upload files to **S3**
2. Launch an **EC2 instance**
3. Install needed tools:

   ```bash
   sudo apt update
   sudo apt install python3-pip
   pip install -r requirements.txt
   ```
4. Run the app on port 8501
5. Open the port in the EC2 security settings

---

## 📏 How We Measure Performance

* **Accuracy** – How often it’s right
* **Precision** – How correct the positive results are
* **Recall** – How many correct results it finds
* **F1 Score** – Balance between precision and recall
* **Response Time** – How fast it gives results

---

## 🔧 Future Ideas

* Use AWS Lambda to reduce costs
* Add support for different languages
* Use live tweets for real-time analysis

---

## 📜 License

This project is under the **MIT License**. You are free to use and modify it.

