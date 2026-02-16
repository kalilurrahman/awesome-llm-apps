# ✨ The Magician IA Reader: AI-Powered NLP & Tarot Insights ✨

Welcome to **The Magician IA Reader**! This project presents a unique application combining the power of Artificial Intelligence with the mystique of tarot reading.

![TheMagicianDemo](https://github.com/maurizioorani/TheMagician-IA-Reader/blob/main/data/readme/TheMagicianAI.gif)

**What it Does:**

This application functions as an AI-driven tarot reader. It takes natural language input and, using an AI model guided by traditional tarot card meanings, provides interpretative insights.


**Key Features:**

* **Natural Language Support:** Understands and interacts in natural language (currently configured for English).
* **Local AI Model ('phi4'):** Runs on the efficient 'phi4' model, ideal for local processing and privacy.
* **CSV-driven Knowledge Base:** Utilizes structured CSV files to store and reference detailed tarot card meanings and symbolism (currently using `data/tarots.csv` with English content).
* **Deep Insights:** Transforms raw text queries into meaningful, context-aware interpretations based on tarot symbolism.

**How it Works:**

The core of The Magician IA Reader lies in its use of the 'phi4' local AI model. This model is fine-tuned or prompted using comprehensive data from CSV files, which contain the interpretations for each tarot card. When a user provides text input, the application processes it through the AI, which then generates a response informed by the tarot meanings.

**Why Use It?**

* **Researchers & Developers:** Explore the capabilities of local AI models for natural language understanding and generation.
* **AI Enthusiasts:** Experiment with a practical application of AI in a unique domain.
* **Curious Minds:** Experience an innovative way to interact with AI for personal insights.

Step into the world where AI meets intuition with The Magician IA Reader!

---

## ⚙️ Installation

#

## Prerequisites

- **Python 3.8 or higher**
- **pip** – Python package installer
- **Ollama** – running locally:
  Install from: https://ollama.com/
  ```bash
  ollama pull phi4
  ollama serve
  ```
  
#

## Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/maurizioorani/TheMagician-IA-Reader.git
   cd TheMagician-IA-Reader
   ```

2. **Set Up a Virtual Environment (Recommended)**

```bash
# On Unix/macOS:
python -m venv venv
source venv/bin/activate


# On Windows:
python -m venv venv
venv\Scripts\activate
```

# Frontend (Streamlit):
First, install all the dependencies
```bash
pip install -r requirements.txt
```

Run the Application

```bash
streamlit run app.py
```
The Streamlit interface will typically be available at http://localhost:8501.

## 📖 How to Use
Access the App: Open your browser and navigate to the URL provided by Streamlit (commonly http://localhost:8501).

Input Your Text Data: Use the intuitive interface to paste, type, or upload the questions you need to be answered.

Choose if you need 3, 5 or 7 cards for the reading.

Read the Insights: View detailed analytics and visualizations that reveal the meaning of the extracted cards.


## 🤝 Contributing
Contributions are welcome! If you have improvements or new features to add, please:

Fork the repository.

Create a new branch for your changes.

Submit a pull request with a clear description of your modifications.

For major changes, please discuss them via an issue before implementation.

## 🛠️ Tech Stack
- Streamlit
- LangChain

## 🚀 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
   cd ./advanced_llm_apps/chat-with-tarots
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```


## 💡 Usage

1. Run the application:
   ```bash
   streamlit run app.py
   ```


## 📸 Screenshots
![data/readme/TheMagicianAI.gif](data/readme/TheMagicianAI.gif)
![images/72-nineofpentacles.jpg](images/72-nineofpentacles.jpg)
![images/29-eightofwands.jpg](images/29-eightofwands.jpg)
![images/19-thesun.jpg](images/19-thesun.jpg)
![images/55-sixofswords.jpg](images/55-sixofswords.jpg)
![images/51-twoofswords.jpg](images/51-twoofswords.jpg)
![images/12-thehangedman.jpg](images/12-thehangedman.jpg)
![images/24-threeofwands.jpg](images/24-threeofwands.jpg)
![images/65-twoofpentacles.jpg](images/65-twoofpentacles.jpg)
![images/41-sixofcups.jpg](images/41-sixofcups.jpg)
![images/11-justice.jpg](images/11-justice.jpg)
![images/69-sixofpentacles.jpg](images/69-sixofpentacles.jpg)
![images/36-aceofcups.jpg](images/36-aceofcups.jpg)
![images/31-tenofwands.jpg](images/31-tenofwands.jpg)
![images/50-aceofswords.jpg](images/50-aceofswords.jpg)
![images/00-thefool.jpg](images/00-thefool.jpg)
![images/21-theworld.jpg](images/21-theworld.jpg)
![images/76-queenofpentacles.jpg](images/76-queenofpentacles.jpg)
![images/42-sevenofcups.jpg](images/42-sevenofcups.jpg)
![images/47-knightofcups.jpg](images/47-knightofcups.jpg)
![images/57-eightofswords.jpg](images/57-eightofswords.jpg)
![images/46-pageofcups.jpg](images/46-pageofcups.jpg)
![images/68-fiveofpentacles.jpg](images/68-fiveofpentacles.jpg)
![images/67-fourofpentacles.jpg](images/67-fourofpentacles.jpg)
![images/14-temperance.jpg](images/14-temperance.jpg)
![images/71-eightofpentacles.jpg](images/71-eightofpentacles.jpg)
![images/10-wheeloffortune.jpg](images/10-wheeloffortune.jpg)
![images/23-twoofwands.jpg](images/23-twoofwands.jpg)
![images/02-thehighpriestess.jpg](images/02-thehighpriestess.jpg)
![images/40-fiveofcups.jpg](images/40-fiveofcups.jpg)
![images/27-sixofwands.jpg](images/27-sixofwands.jpg)
![images/75-knightofpentacles.jpg](images/75-knightofpentacles.jpg)
![images/08-thestrength.jpg](images/08-thestrength.jpg)
![images/48-queenofcups.jpg](images/48-queenofcups.jpg)
![images/07-thechariot.jpg](images/07-thechariot.jpg)
![images/77-kingofpentacles.jpg](images/77-kingofpentacles.jpg)
![images/64-aceofpentacles.jpg](images/64-aceofpentacles.jpg)
![images/60-pageofswords.jpg](images/60-pageofswords.jpg)
![images/30-nineofwands.jpg](images/30-nineofwands.jpg)
![images/63-kingofswords.jpg](images/63-kingofswords.jpg)
![images/04-theemperor.jpg](images/04-theemperor.jpg)
![images/73-tenofpentacles.jpg](images/73-tenofpentacles.jpg)
![images/09-thehermit.jpg](images/09-thehermit.jpg)
![images/06-thelovers.jpg](images/06-thelovers.jpg)
![images/05-thehierophant.jpg](images/05-thehierophant.jpg)
![images/17-thestar.jpg](images/17-thestar.jpg)
![images/58-nineofswords.jpg](images/58-nineofswords.jpg)
![images/32-pageofwands.jpg](images/32-pageofwands.jpg)
![images/26-fiveofwands.jpg](images/26-fiveofwands.jpg)
![images/44-nineofcups.jpg](images/44-nineofcups.jpg)
![images/74-pageofpentacles.jpg](images/74-pageofpentacles.jpg)
![images/37-twoofcups.jpg](images/37-twoofcups.jpg)
![images/70-sevenofpentacles.jpg](images/70-sevenofpentacles.jpg)
![images/62-queenofswords.jpg](images/62-queenofswords.jpg)
![images/59-tenofswords.jpg](images/59-tenofswords.jpg)
![images/18-themoon.jpg](images/18-themoon.jpg)
![images/25-fourofwands.jpg](images/25-fourofwands.jpg)
![images/03-theempress.jpg](images/03-theempress.jpg)
![images/22-aceofwands.jpg](images/22-aceofwands.jpg)
![images/52-threeofswords.jpg](images/52-threeofswords.jpg)
![images/16-thetower.jpg](images/16-thetower.jpg)
![images/56-sevenofswords.jpg](images/56-sevenofswords.jpg)
![images/35-kingofwands.jpg](images/35-kingofwands.jpg)
![images/33-knightofwands.jpg](images/33-knightofwands.jpg)
![images/15-thedevil.jpg](images/15-thedevil.jpg)
![images/43-eightofcups.jpg](images/43-eightofcups.jpg)
![images/45-tenofcups.jpg](images/45-tenofcups.jpg)
![images/34-queenofwands.jpg](images/34-queenofwands.jpg)
![images/53-fourofswords.jpg](images/53-fourofswords.jpg)
![images/66-threeofpentacles.jpg](images/66-threeofpentacles.jpg)
![images/28-sevenofwands.jpg](images/28-sevenofwands.jpg)
![images/54-fiveofswords.jpg](images/54-fiveofswords.jpg)
![images/49-kingofcups.jpg](images/49-kingofcups.jpg)
![images/01-themagician.jpg](images/01-themagician.jpg)
![images/38-threeofcups.jpg](images/38-threeofcups.jpg)
![images/20-judgement.jpg](images/20-judgement.jpg)
![images/39-fourofcups.jpg](images/39-fourofcups.jpg)
![images/13-death.jpg](images/13-death.jpg)
![images/61-knightofswords.jpg](images/61-knightofswords.jpg)
