# 🧠 GPT-2 FOMC Text Generator

This is a project where we teach a LLM (GPT-2) to write like the US Federal Reserve! 

## 📚 What is this project?

* The US Fed (Federal Reserve) writes serious economic reports called **FOMC Meeting Minutes**.
* We used those reports to train a computer model (GPT-2).
* After training, the model can **write similar text** in the same serious tone (called "Fed-speak").

## 📂 What’s inside this project?

* `Fed_Scrape-2015-2023.csv` → A file with real FOMC meeting sentences.
* `gpt-2-FOMC.h5` → The trained GPT-2 model (so you don’t have to train again).
* `fomc-statement-generation-gpt-2(1).ipynb` → The code notebook where everything happens (training + testing).
* `BTP_Report.pdf` → A full report if you want to learn how we did it, step-by-step.
* `btp.pptx` → Presentation slides summarizing the project.
* `requirements.txt` → List of Python libraries needed to run this project.
* `demo.gif` → A GIF showing how the model generates text.

## 🛠️ Tools Used

* **Python** (the main language)
* **Hugging Face Transformers** (for GPT-2 model)
* **PyTorch, Pandas, NumPy** (to help with training and data)

## 🧪 What the model does

You give it a sentence like:

> "The Federal Reserve decided to..."

And the model continues with:

> "...increase the interest rate by 25 basis points to support economic growth."

💡 Cool, right?

## 🎯 Why this project is useful?

* Helps students learn how to fine-tune AI.
* Shows how AI can write like experts (even in finance).
* Fun way to mix **AI + Economics**!

## 🚀 How to run this

### 🔁 Option 1: Run on Google Colab (easiest)

1. Open the `.ipynb` file in Google Colab.
2. Run the code step by step.
3. Try your own sentence prompts.

### 💻 Option 2: Run Locally (on your own computer)

#### 🧰 Step 1: Install Python (if not already)

Make sure Python 3.8+ is installed. You can check with:

```bash
python --version
```

#### 🧪 Step 2: Set up virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # for Linux/Mac
venv\Scripts\activate     # for Windows
```

#### 📦 Step 3: Install required packages

```bash
pip install -r requirements.txt
```

If there's no `requirements.txt`, install manually:

```bash
pip install torch transformers pandas numpy matplotlib jupyter
```

#### 📁 Step 4: Open the Jupyter Notebook

```bash
jupyter notebook fomc-statement-generation-gpt-2(1).ipynb
```

#### 🤖 Step 5: Run the notebook step-by-step

* The notebook loads the GPT-2 model.
* Fine-tunes it using the data in `Fed_Scrape-2015-2023.csv`.
* You can also load the already trained model (`gpt-2-FOMC.h5`) and generate text directly.

## 📌 Tips

* If you see memory errors, try reducing batch size or sequence length.
* Use GPU if available for faster training (Colab is great for that).



## 🙋‍♂️ Made by

**Divyansh Gupta**
Rajiv Gandhi Institute of Petroleum Technology
May 2025

