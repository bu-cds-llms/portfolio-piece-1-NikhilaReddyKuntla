# 📊 LLM Token & Cost Analyzer

An interactive Jupyter/Colab dashboard designed to estimate costs and analyze text diversity for OpenAI models. This tool provides real-time tokenization insights, cost projections, and visual data representations.

## 🚀 Features

* **Real-time Tokenization:** Uses OpenAI's `tiktoken` library to accurately count tokens for specific models (GPT-3.5-Turbo and GPT-4).
* **Cost Estimation:** Calculates the approximate API cost based on the token pricing.
* **Text Diversity Analysis:** Computes the ratio of unique words to total word count to identify repetitive vs. diverse content.
* **Interactive UI:** Built with `ipywidgets` for a seamless, "app-like" experience inside a notebook.
* **Visual Analytics:** Automatically generates a comparison bar chart of Words vs. Tokens using `matplotlib`.

## 🛠️ Tech Stack

* **Language:** Python
* **Tokenization:** [tiktoken](https://github.com/openai/tiktoken)
* **Visualization:** Matplotlib
* **UI Components:** IPyWidgets
* **Environment:** Jupyter Notebook / Google Colab

## 📦 Installation

To run this dashboard locally, ensure you have Python installed and run:

```bash
pip install tiktoken matplotlib ipywidgets

```

## 🖥️ Usage

1. Open the `Portfolio.ipynb` notebook in Google Colab or a local Jupyter server.
2. Run all cells to initialize the dashboard.
3. **Input Text:** Paste your prompt or document into the text area.
4. **Select Model:** Choose between `gpt-3.5-turbo` or `gpt-4` from the dropdown.
5. **Analyze:** Click the **Analyze 🚀** button.

### Example Output

> **✨ LLM TEXT ANALYSIS DASHBOARD**
> * **Words:** 8
> * **Tokens:** 10
> * **Cost:** $0.000020
> * **Insights:** High diversity text / Small input (cheap & fast)
> 
> 

## 📊 Logic & Pricing

The analyzer uses the following (approximate) pricing per 1,000 tokens:

* **GPT-3.5-Turbo:** $0.002
* **GPT-4:** $0.03

---

**Note:** *This project is intended for estimation purposes. Actual OpenAI API billing may vary based on specific model versions and usage tiers.*
