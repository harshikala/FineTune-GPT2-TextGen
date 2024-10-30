# FineTune-GPT2-TextGen

This project fine-tunes OpenAI’s GPT-2 model to generate text in the style of Shakespeare. Leveraging a custom dataset (`shakespeare.txt`) and the Hugging Face Transformers library, the model is trained to produce coherent and contextually relevant text that emulates Shakespeare’s writing style. Through extensive experimentation, this project implements nuanced text generation techniques, such as top-k and top-p sampling, to improve the output quality. This repository includes scripts for loading models, tokenizing data, generating text sequences, and configuring generation parameters.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Training Process](#training-process)
6. [Text Generation](#text-generation)
7. [Results](#results)
8. [Acknowledgments](#acknowledgments)

---

## Project Overview

The **GPT2-Shakespeare-Generator** project was developed to explore fine-tuning methods for transforming GPT-2 into a Shakespearean text generator. Starting with data processing, tokenization, and model setup, this project uses a custom dataset and applies advanced text generation settings to create outputs reflective of the dataset’s language style. The model uses a combination of top-k and top-p sampling for more sophisticated text generation.

## Features

- **Custom Dataset**: Fine-tunes GPT-2 with a Shakespeare-style dataset.
- **Data Handling**: Loads and processes PDFs, Word documents, and text files.
- **Text Generation Settings**: Uses advanced sampling techniques like top-k and top-p for refined outputs.
- **Token and Padding Management**: Sets EOS token as the pad token for efficient batch processing.
- **Reusable Code Functions**: Modular functions for loading models, tokenizing data, and generating text sequences.

## Installation

Clone the repository and install the required dependencies.

```bash
git clone 'https://github.com/harshikala/FineTune-GPT2-TextGen.git'
```

## Usage
1. **Data Preparation**: Place your custom dataset in the /data directory.
2. **Model Training**: Run train_model.py with the necessary parameters to fine-tune GPT-2.
3. **Generate Text**: Use generate_text.py to produce Shakespeare-style text from the fine-tuned model.

## Training Process
The training process involves loading a pre-trained GPT-2 model and fine-tuning it with the shakespeare.txt dataset. Parameters like batch size, epochs, and save steps can be adjusted in train_model.py.

## Text Generation
Text generation leverages top-k and top-p sampling for nuanced outputs. The model can be tested with custom input prompts to generate stylistically accurate text in response.

## Results
The fine-tuned model generates coherent text with contextual relevance, closely resembling the writing style of the provided dataset. Outputs can be further customized with generation parameters for specific tasks.

## Acknowledgments
Special thanks to Hugging Face for providing an accessible library for model fine-tuning.
