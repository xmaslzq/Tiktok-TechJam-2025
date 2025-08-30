# Tiktok-TechJam-2025 (Team 1+1=3)

## 📌 Problem Statement
Location-based review platforms such as Google Maps often face the challenge of **low-quality, irrelevant, or misleading reviews**.  
Many reviews are:
- Advertisements  
- Vague one-liners  
- Written by people who have **never visited** the location  

These undermine trust and make it difficult for genuine users to assess the quality of a place.  

**Hence the problem statement arises:**  
We focus on filtering out **ads, irrelevant content, non-visit reviews, and vague/low-information comments** to ensure that users and businesses alike benefit from authentic and trustworthy feedback.  

--
## 🚀 Solution Overview
We developed an **OpenAI-powered review evaluation system** that automatically analyzes comments and flags those that are likely to be untrustworthy or irrelevant.  

The solution works by combining **natural language processing (NLP)** with **machine learning classification**, using both:  
- **Rule-based heuristics** (keyword patterns, URL detection, vagueness filters)  
- **LLM-powered reasoning** (GPT-4o for contextual understanding)  

Afterwards, we also applied **clustering per company** to classify and remove anomalies, ensuring more reliable and trustworthy results.  

---

## ✨ Key Features
- **Multi-criteria classification**: Detects Ads, Irrelevant content, Non-visit indicators, and Vagueness.  
- **Hybrid evaluation approach**: Combines heuristics (e.g., promotional keywords) with LLM contextual checks.  
- **Quality & Relevance scoring**: Assigns each review a score reflecting its usefulness.  
- **Customizable output**: Provides structured JSON/CSV output for dashboards or third-party apps.  
- **Scalable design**: Built to handle large batches of reviews efficiently.  

---

## 🎯 How It Solves the Problem
- **Trustworthiness**: Filters out misleading or spam reviews, ensuring only genuine feedback is highlighted.  
- **Relevance**: Identifies whether the comment is truly based on a real visit experience.  
- **Reliability**: Uses clustering to detect anomalies and reduce bias across different businesses.  

---

## 🛠️ Development Tools
- **Google Colab** – For experimentation, model fine-tuning, and dataset preprocessing.  
- **Visual Studio Code** with Conda environment – For statistical analysis and showcasing results.  
> _(Model is still in experimentation stage; not yet migrated fully to main IDE.)_  

---

## 🔗 APIs Used
- **OpenAI GPT-4o** – For natural language classification and nuanced contextual understanding.  

---

## 📚 Libraries & Frameworks
- **Python (core language)**  
- **pandas & numpy** – Data preprocessing and manipulation  
- **scikit-learn** – ML classifiers and evaluation metrics  
- **Hugging Face Transformers** – For fine-tuning NLP models where required  
- **PyTorch** – Model training and inference  
- **Regex** – Heuristic text pattern matching (ads, links, promo keywords)  
- **tldextract** – Accurately separates URL subdomain, domain, and public suffix using PSL  
- **backoff** – Retry failed API attempts with exponential backoff delays  
- **tqdm** – Progress tracking for AI batch processing  
- **matplotlib & seaborn** – Graph plotting, diagrams, and visualization  

---

## 📊 Assets & Datasets
- **Google Review Data**: Open datasets containing Google location reviews  
  - Example: [Google Maps Restaurant Reviews on Kaggle](https://www.kaggle.com/datasets/denizbilginn/google-maps-restaurant-reviews)  

---

## ⚡ Setup Guide
### 1. Bring the code to Google Colab
### 2. Import the dataset in csv file ("reviews.csv") at contents folder
### 3. Setup OpenAPI Secret Key
  - named it OPENAI_API_KEY
## Then Run

---
## Contribution
- Yu Yue (Statisics part)
- Li Zhi Qi (AI part)
