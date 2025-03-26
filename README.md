# AI Recipe Generator

## Overview

The AI Recipe Generator is a deep learning model that generates custom recipes based on user prompts. It utilizes a **T5 transformer model** fine-tuned on a recipe dataset to generate structured ingredient lists and cooking directions.

## Features

- Generates recipes based on user-defined prompts (e.g., "Make a vegan pasta recipe").
- Fine-tuned **T5 transformer model** for high-quality text generation.
- **Data preprocessing**: Cleaning, tokenization, and train-test split.
- **Performance evaluation** using **BLEU, ROUGE, and Perplexity** scores.

## Dataset

The model is trained on a **Kaggle recipe dataset**, which includes:

- **Prompt (input):** User query (e.g., "Make a chocolate cake").
- **Recipe (output):** Ingredients and step-by-step instructions.

## Model Training

The training process includes:

1. **Data Preprocessing**: Text normalization, tokenization, and padding.
2. **Fine-tuning the T5 Model**:
   - **Training epochs:** 5
   - **Batch size:** 8
   - **Optimizer:** AdamW with weight decay
   - **Learning rate scheduler** with warm-up steps
3. **Evaluation Metrics**:
   - **BLEU Score**: Measures similarity to reference text.
   - **ROUGE Score**: Evaluates text overlap.
   - **Perplexity**: Measures text prediction quality.

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/AI-Recipe-Generator.git
cd AI-Recipe-Generator
pip install -r requirements.txt
```

## Usage

Run the script to generate recipes:

```bash
python generate_recipe.py --prompt "Make a healthy smoothie"
```

## Technologies Used

- **Python**
- **TensorFlow / PyTorch**
- **Hugging Face Transformers**
- **NLP (Natural Language Processing)**
- **BLEU & ROUGE evaluation metrics**

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

## License

This project is licensed under the MIT License.

## Contact

**Author\:Sushant Kumar Pal**\
**Email:** 2021ucp1094\@mnit.ac.in\
**Institution:** MNIT Jaipur

