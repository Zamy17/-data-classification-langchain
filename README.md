# 🤖 NLP Review Classification & Personality Analysis using LangChain + Google Colab

> 🚀 This project is a beginner-level exploration in **Natural Language Processing (NLP)**, **Data Classification**, and **LLM-powered Extraction** using LangChain (Replicate API) in Google Colab.

---

## 📌 Project Summary

This project demonstrates how to:

- 🔍 Classify customer reviews as **Positive**, **Negative**, or **Mixed**
- 🧠 Extract structured data like **name**, **age**, and **job** from free-form tex
- 📊 Perform basic **Exploratory Data Analysis (EDA)** on a personality dataset
- 🎨 Visualize time spent alone by **Introverts vs Extroverts**

All experiments were run in Google Colab using Python, LangChain, and open-source libraries.

---

## 🧰 Tools & Technologies Used

| Tool | Description |
|------|-------------|
| 🐍 Python | Programming language |
| 🧠 LangChain + Replicate | LLM interaction |
| 📚 pandas | Data analysis |
| 📈 seaborn, matplotlib | Visualization |
| 🧪 Google Colab | Interactive notebook |
| 💻 GitHub | Version control & portfolio |

---

## 📁 File Structure

📦 data-classification-langchain/
├── sdi_data_session_2_m_zam_zami.py # Python script exported from Google Colab
├── README.md # This markdown file


---
## 📊 Sample Visualization

![Introvert vs Extrovert Visualization](https://raw.githubusercontent.com/Zamy17/-data-classification-langchain/main/introvert_vs_extrovert.png)

---
## 💡 Key Code Examples
---
### ✅ Review Classification with LLM
```python
prompt = f"""
Classify this review as Positive, Negative, Mixed. Respond with label only.
{review}
"""
ai_output = llm.invoke(prompt)
print("AI Output:", ai_output)

🧾 Extract Name, Age, Job from Sentence

prompt = f"""
Please extract the data and get name, age, and job. Output in JSON.
{row}
"""
ai_output = llm.invoke(prompt)
print("AI Output:", ai_output)

📊 Plot Introvert vs Extrovert Time

sns.barplot(x=['Introvert', 'Extrovert'], y=[avg_alone_intro, avg_alone_extro])
plt.title('Average Alone Time: Introvert vs Extrovert')
