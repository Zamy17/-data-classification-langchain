🤖 NLP Review Classification & Personality Analysis with LangChain & Google Colab

A beginner-level project for exploring Natural Language Processing (NLP), data classification, and LLM-powered information extraction — powered by LangChain (via Replicate API) and visualized in Python.

📝 Project Overview

This repository contains an end-to-end mini project demonstrating:

🔍 Sentiment classification of customer reviews (Positive / Negative / Mixed)

🧠 Information extraction (name, age, job) from descriptive sentences

📊 Exploratory Data Analysis (EDA) on personality datasets

📈 Visualization: comparing average time spent alone by introverts vs extroverts

The code was written and tested in Google Colab and exported as a .py script.

🧰 Tools & Technologies

Tool

Purpose

Python 🐍

Core programming language

LangChain 🧠

LLM framework for Replicate

Replicate API 🔁

Access to large language models

pandas 📚

Data analysis & wrangling

seaborn & matplotlib 📊

Visualization

Google Colab ☁️

Experimentation environment

GitHub 💻

Version control & portfolio

📁 File Structure

📆 data-classification-langchain/
🔹 sdi_data_session_2_m_zam_zami.py   # Main Python script from Google Colab
🔹 README.md                          # Project documentation (this file)

💡 Key Features & Examples

✅ Sentiment Classification Prompt

prompt = f"""
Classify this review as Positive, Negative, or Mixed. Respond with label only.
{review}
"""
ai_output = llm.invoke(prompt)
print("AI Output:", ai_output)

🢾 Information Extraction from Text

prompt = f"""
Please extract name, age, and job from the sentence. Output in JSON.
{row}
"""
ai_output = llm.invoke(prompt)
print("AI Output:", ai_output)

📈 Personality Comparison (Introvert vs Extrovert)

sns.barplot(x=['Introvert', 'Extrovert'], y=[avg_alone_intro, avg_alone_extro])
plt.title('Average Time Alone: Introvert vs Extrovert')
plt.ylabel('Hours per Day')

📊 Sample Visualization

(You can replace this with a real image of your plot if uploaded)



🌟 Learning Goals

Through this project, I learned how to:

Utilize LLMs via LangChain & Replicate API for classification and extraction

Process and analyze real-world datasets using pandas

Create clean and meaningful visualizations using seaborn/matplotlib

Structure code for public sharing in a GitHub portfolio

👨‍💻 About Me

M. Zam ZamiAspiring Data Analyst & NLP Enthusiast
