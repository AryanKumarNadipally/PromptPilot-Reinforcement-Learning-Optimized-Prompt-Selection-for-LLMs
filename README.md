# PromptPilot: Reinforcement Learning-Optimized Prompt Selection for LLMs

PromptPilot is a demo project under development that automates prompt engineering for Large Language Models (LLMs) using Reinforcement Learning (RL). It optimizes prompt selection to generate high-quality, concise, and context-aware responses. The system leverages Cerebras' fast inference for efficiency, enabling rapid testing and training cycles.

---

## 🚀 Features

- **Reinforcement Learning:** Uses Proximal Policy Optimization (PPO) for optimal prompt selection.
- **Semantic Scoring:** Measures output quality with SentenceTransformer-based semantic similarity.
- **Dynamic Refinement:** Multi-step RL episodes allow iterative prompt optimization.
- **Cerebras Integration:** Fast inference via Cerebras LLM models for rapid training and scalability.
- **Interactive Interface:** Gradio-powered interface for user-friendly demonstrations.

---

## 🛠️ Setup Instructions

This project runs on Google Colab for ease of access. Follow the steps below to set it up and run the demonstration:

### 1. Clone or Download the Repository
Download or clone this repository to get all the required files, including the `.ipynb` notebook and necessary datasets:
```bash
git clone https://github.com/yourusername/PromptPilot.git
```

### 2. Open the Notebook in Google Colab
- Upload the `PromptPilot.ipynb` file to your Google Drive.
- Open the file in Google Colab.

---

## 📂 Upload Required Files

### Files Needed:
1. **`questions_dataset.json`**: Contains the list of questions and gold-standard answers.
2. **`config.json`**: Stores your Cerebras API key.

### How to Upload Files:
1. In the Google Colab sidebar, go to the **File** section.
2. Use the **Upload button** to upload the `questions_dataset.json` and `config.json` files to the working directory.

---

## 📝 Set Up the API Key

1. Open the `config.json` file in any text editor.
2. Replace the placeholder text with your Cerebras API key:
   ```json
   {
       "api_key": "your-cerebras-api-key"
   }
   ```
3. Save the file.
4. Upload the updated `config.json` file to the Colab environment.

---

## ▶️ Running the Notebook

Once the files are uploaded and the API key is configured:
1. Run each cell sequentially in the notebook.
2. The notebook will:
   - Load the dataset and config files.
   - Train an RL agent using PPO on the prompt variants.
   - Launch an interactive Gradio interface for testing.

---

## 💻 Gradio Demo

The Gradio interface allows you to:
1. Select a question from the dataset.
2. View the RL agent's selected prompt variant.
3. See the LLM's response to the optimized prompt.

---

## 🛣️ Future Development

This project is currently under active development. Planned improvements include:
- Creating a Chrome extension for seamless prompt optimization.
- Deploying as a standalone Gradio-powered web application.
- Adding real-time LLM queries for dynamic environments.
- Integrating domain-specific optimizations for healthcare, legal, and academic use cases.

---

## 📧 Contact

For questions or feedback, reach out to:
- **Name:** Aryan Kumar Nadipally
- **Email:** anadipa1@asu.edu 
- **LinkedIn:** (https://www.linkedin.com/in/aryan-kumar-nadipally/)

---

### ⚠️ Disclaimer

This is a demonstration project. The system relies on pre-fetched LLM responses and cached data for cost efficiency in training. Future iterations will include real-time LLM interaction capabilities.
