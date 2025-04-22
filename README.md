<h1 align="center">👋 Hey there, I'm Mohammad Shan!</h1>
<p align="center">🚀 AI Explorer | 🎵 Song Classifier Builder | 🧠 Machine Learning Enthusiast</p>

<p align="center">
  <img src="https://media.giphy.com/media/your-gif-link-here.gif" alt="AI Music Demo" width="600"/>
</p>

---

### 🔍 About Me

- 🎓 Passionate learner & developer diving deep into **AI & Machine Learning**
- 🎧 Built a deep learning app that detects whether a song is **AI-generated or human-written**
- 🧪 Experimenting with **LSTM**, **CNNs**, and **speech recognition models**
- 🌱 Currently exploring: **Transformers**, **Flask App Deployment**, and **Explainable AI**

---

### 💡 Tech Stack & Tools

![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![SpeechRecognition](https://img.shields.io/badge/SpeechRecognition-FFD43B?style=for-the-badge&logo=google&logoColor=black)
![VS Code](https://img.shields.io/badge/VSCode-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

---

### 🚀 Projects I'm Proud Of

- 🎤 **AI vs Real Song Classifier**  
  Deep learning model + Flask app that analyzes audio and predicts if the lyrics are AI-generated or written by a human.

- 🧠 **ML & Deep Learning Notebooks**  
  Exploratory projects using **Random Forest**, **LSTM**, **Transformers**, and more.

- 💬 **Speech-to-Text Tools**  
  Custom pipeline for converting songs or speech into text for NLP tasks.

---

### 📫 Let's Connect!

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-blue?style=for-the-badge&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/mohammad-shan-026149360/?originalSubdomain=in)
[![Gmail](https://img.shields.io/badge/-Email-D14836?style=for-the-badge&logo=Gmail&logoColor=white)](mailto:mohammadshan123@gmail.com)
[![GitHub](https://img.shields.io/badge/-GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mohammadshan123)

---

### ⚡ Fun Fact

> I turned a **musical curiosity** into a **machine learning challenge**, and built a model that listens to lyrics and says:  
> “Nah, that one’s too robotic. Must be AI.” 🤖🎵

---

<!---
mohammadshan123/mohammadshan123 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

name: Generate Snake Animation

on:
  schedule:
    - cron: "0 */12 * * *"  # Runs every 12 hours
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Generate Snake Animation
        uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
            dist/github-contribution-grid-snake.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9

      - name: Deploy to GitHub Pages
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/mohammadshan123/mohammadshan123/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/mohammadshan123/mohammadshan123/output/github-contribution-grid-snake.svg" />
  <img alt="github-snake" src="https://raw.githubusercontent.com/mohammadshan123/mohammadshan123/output/github-contribution-grid-snake.svg" />
</picture>

