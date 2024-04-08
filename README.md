# AllyArc ML Component

## Overview

The AllyArc project leverages conversational AI to create an engaging and supportive educational experience for autistic learners. This repository contains the development lifecycle of the AllyArc chatbot, from dataset creation, through model fine-tuning, to performance evaluation. Initially, the project explored the use of the LLaMA model, but due to limitations in conversational capabilities, it pivoted to the GPT-3.5 Turbo model.

## Getting Started

To replicate or build upon this project, you will need:
- Python 3.8 or later
- Access to Hugging Face and OpenAI APIs
- Jupyter Notebook or JupyterLab

First, clone this repository to your local machine:

```bash
git clone https://github.com/yourgithubusername/allyarc-project.git
cd allyarc-project
```

Install the required Python packages:

```bash
pip install -r requirements.txt
```

## Notebooks Description & Setup

### 1. `AllyArc_Dataset_Chat.ipynb`

#### Purpose
Initial dataset construction for the chatbot.

#### Setup
Ensure you have Jupyter Notebook installed and run:

```bash
jupyter notebook AllyArc_Dataset_Chat.ipynb
```

#### Description
This notebook outlines the steps to compile and preprocess the initial dataset. Follow the instructions within to generate your dataset.

#### Output
Dataset uploaded to Hugging Face: [AllyArc/chat_dataset](https://huggingface.co/datasets/AllyArc/chat_dataset).

### 2. `Share_FineTuneAllyArc_llama.ipynb`

#### Purpose
Fine-tuning the LLaMA model with the prepared dataset.

#### Setup
Launch this notebook in Jupyter:

```bash
jupyter notebook Share_FineTuneAllyArc_llama.ipynb
```

#### Description
Details the process of fine-tuning the LLaMA model. Execute each cell as per the instructions provided within.

#### Output
Fine-tuned model on Hugging Face: [AllyArc/llama_allyarc](https://huggingface.co/AllyArc/llama_allyarc).

### 3. `AllyArc_Dataset_OAI_Format.ipynb`

#### Purpose
Reformatting the dataset for GPT-3.5 Turbo model fine-tuning.

#### Setup
Run the notebook via Jupyter:

```bash
jupyter notebook AllyArc_Dataset_OAI_Format.ipynb
```

#### Description
Adjusts the dataset structure for OpenAI model compatibility. Follow the notebook steps to modify and export your dataset.

#### Output
Reformatted dataset on Hugging Face: [AllyArc/allyarc_oai_format](https://huggingface.co/datasets/AllyArc/allyarc_oai_format).

### 4. `check_format.ipynb`

#### Purpose
Validate the dataset format for OpenAI fine-tuning.

#### Setup
Execute the notebook in Jupyter:

```bash
jupyter notebook check_format.ipynb
```

#### Description
Ensures the dataset is correctly formatted for fine-tuning. Execute the cells and follow any corrective actions suggested.

### 5. `eval_oai.ipynb`

#### Purpose
Evaluate the fine-tuned GPT-3.5 Turbo model's performance.

#### Setup
Launch with Jupyter:

```bash
jupyter notebook eval_oai.ipynb
```

#### Description
This notebook assesses the fine-tuned model using specific prompts. Follow the notebook to run the evaluation and view the results.

## Contributing

We welcome contributions to the AllyArc project. Please open an issue to discuss your ideas or submit pull requests for consideration.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
