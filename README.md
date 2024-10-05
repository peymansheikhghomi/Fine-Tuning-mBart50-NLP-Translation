# Fine-Tuning mBart50 for NLP-Based English-Persian Subtitle Translation

This repository contains notebooks for fine-tuning the [mBart 50 model](https://arxiv.org/abs/2008.00401) for translating English subtitles into Persian. The project leverages the capabilities of the [Hugging Face Transformers](https://huggingface.co/) library to create an effective translation tool.

## Overview

The project consists of two main functionalities:

1. **Fine-Tuning mBart 50 for English-Persian Subtitle Translation:**
   - This notebook demonstrates the process of fine-tuning the pre-trained mBart 50 model on a [dataset of English-Persian subtitle pairs](https://huggingface.co/datasets/Peymansoft/English-Persian-Subtitle). It covers data loading, tokenization, model training, evaluation, and inference.
   - [The fine-tuned model has been made available on Hugging Face](https://huggingface.co/Peymansoft/MBart-50-Subtitle-English-Persian) for open-source access and further development by the community.

2. **Leveraging the Fine-Tuned Model for Translation:**
   - This notebook showcases the practical application of the fine-tuned model. It features two interactive functionalities:
     - **Subtitle Translation:** Users can upload English SRT subtitle files to receive translated Persian SRT subtitles.
     - **Sentence Translation:** Users can input arbitrary English sentences to compare translation results before and after fine-tuning.

## Results

### Before and After Fine-Tuning

Here are a few examples of translations before and after the fine-tuning process:

| English Sentence                        | Translation Before Fine-Tuning        | Translation After Fine-Tuning         |
|-----------------------------------------|---------------------------------------|---------------------------------------|
| "Hello you guys, what's up?" |"سلام بچه ها ، چیه ؟"|"سلام بچه ها، چه خبر؟"
| "Toto, I've a feeling we're not in Kansas anymore." | "توتو، من احساسی دارم که دیگر در کانزاس نیستیم." | "توتو، حس می‌کنم که دیگر در کانزاس نیستیم." |
|"m gonna make him an offer he can't refuse"|"من به او پیشنهادی می دهم که او نمی تواند رد کند"|"من به اون پیشنهادی میدم که اون نمیتونه رد کنه"|

## Requirements

To run the notebooks, you will need the following dependencies:

- Python 3.x
- `datasets`
- `srt`
- `transformers`
- `gradio`
- `evaluate` (for evaluation metrics)

You can install these dependencies using pip:

```bash
pip install datasets srt transformers gradio evaluate
```
## Usage

### Fine-Tuning mBart 50

1. Open the notebook `Fine-Tuning mBart for English to Persian Subtitle Translation.ipynb`.
2. Follow the instructions to load the dataset, preprocess the data, fine-tune the model, and evaluate its performance.

### Subtitle Translation

1. Open the notebook `Leveraging Fine-Tuned mBart 50 for English-Persian Subtitle Translation.ipynb`.
2. Use the subtitle translation feature to upload an English SRT file and download the translated Persian subtitles.
3. Use the sentence translation feature to input English sentences and compare translations before and after fine-tuning.

## Contributions

Contributions to improve the model and enhance its functionalities are welcome! Please feel free to open issues or submit pull requests.

## Acknowledgments

- [Hugging Face](https://huggingface.co/) for providing the Transformers library and model hub.
- The community for their contributions and support in developing machine translation models.
