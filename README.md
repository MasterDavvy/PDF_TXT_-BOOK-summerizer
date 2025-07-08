# PDF/TXT Summarizer using OpenRouter and LLaMA-4 Maverick

This repository contains a Google Colab notebook that summarizes PDF or TXT files using a large language model via OpenRouter’s API. The default model is "meta-llama/llama-4-maverick", but users can select any supported OpenRouter model during execution.

## Features

- Upload PDF or TXT files directly in Colab
- Choose between bullet-point or paragraph-style summaries
- Customize chunk size for processing large documents
- Download the generated summary as a TXT file
- Interactive model selection (default: "meta-llama/llama-4-maverick")

## Requirements

- A Google account to use Google Colab
- An OpenRouter API key (free to sign up)

## Setup

For detailed instructions on obtaining an OpenRouter API key and selecting a model, see [SETUP.md](SETUP.md). Key steps include:
- Sign up at [OpenRouter.ai](https://openrouter.ai) and generate an API key.
- Verify available models at [OpenRouter Models](https://openrouter.ai/models).

## Running the Notebook

1. Open the notebook in Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yourusername/yourrepo/blob/main/summarizer.ipynb)
2. Run the first cell to install dependencies.
3. Enter your OpenRouter API key when prompted.
4. Configure settings:
   - **Model**: Press Enter for the default ("meta-llama/llama-4-maverick") or enter another model ID from OpenRouter.
   - **Chunk Size**, **Summary Style**, and **Output File Name**: Follow the prompts to customize.
5. Upload a PDF or TXT file when prompted.
6. Run all cells to generate and download the summary.

**Note**: Replace `yourusername/yourrepo` in the "Open in Colab" badge with your actual GitHub username and repository name.

## Directory Structure

- `summarizer.ipynb`: The main Colab notebook for summarizing documents
- `README.md`: This file
- `SETUP.md`: Detailed setup instructions, including how to obtain the API key and select models

## Notes

- Ensure the selected model is valid by checking [OpenRouter Models](https://openrouter.ai/models).
- Some models may require credits or have specific token limits, which can affect summarization performance.