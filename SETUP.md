# Setup Guide for PDF/TXT Summarizer

This guide provides detailed instructions on how to set up and use the PDF/TXT summarizer notebook in Google Colab.

## 1. Sign Up for OpenRouter

To use this notebook, you need an OpenRouter API key. Follow these steps to obtain one:

1. Visit [OpenRouter.ai](https://openrouter.ai).
2. Click "Sign Up" or "Get Started" and create an account using your email or a supported authentication method.
3. Log in to your OpenRouter account.
4. Navigate to the "API Keys" section (typically found in your profile or settings dashboard).
5. Generate a new API key or copy an existing one.
6. Securely store the API key, as you’ll need to paste it into the notebook when prompted.

## 2. Select a Model

The notebook defaults to the "meta-llama/llama-4-maverick" model for summarization, but you can choose any model supported by OpenRouter. Here’s how:

- **Default Model**: The notebook uses "meta-llama/llama-4-maverick" by default. If you press Enter at the model prompt, this model will be used.
- **Changing the Model**: When running the notebook, you’ll be prompted to enter a model name. You can input any valid model ID from OpenRouter, such as `gryphe/mythomax-l2-13b` or `anthropic/claude-3.5-sonnet`.
- **Finding Model IDs**: Visit [OpenRouter Models](https://openrouter.ai/models) to see the list of available models and their IDs.
- **Important**: Verify that the model you choose is active and supported by OpenRouter. Some models may require additional credits or have specific token limits. Check the model details on OpenRouter’s website to ensure compatibility.

## 3. Running the Notebook in Colab

1. Open the notebook in Google Colab using the "Open in Colab" badge in the [README.md](README.md) or by uploading `summarizer.ipynb` to your Google Drive and opening it in Colab.
2. Run the first cell to install required libraries (`openai`, `pdfplumber`, `tqdm`).
3. When prompted, enter your OpenRouter API key.
4. Configure the summarization settings:
   - **Model**: Press Enter to use the default ("meta-llama/llama-4-maverick") or enter a different model ID from OpenRouter.
   - **Chunk Size**: Set the token size for splitting the document (default: 2000 tokens). Adjust based on document length or model limits.
   - **Summary Style**: Choose "bullets" or "paragraph" (default: bullets).
   - **Output File Name**: Specify the name for the summary file (default: "summary").
5. Upload a PDF or TXT file when prompted by the notebook.
6. Run all cells to process the file, generate the summary, and download it as a TXT file.

## 4. Troubleshooting

- **API Key Issues**:
  - Ensure your API key is correct and active in your OpenRouter account.
  - Check for usage limits or credit requirements on OpenRouter (some models may require credits for heavy use).
- **Model Selection**:
  - If you encounter errors, verify that the model ID is valid by checking [OpenRouter Models](https://openrouter.ai/models).
  - Ensure the model supports text summarization and is compatible with the notebook’s settings (e.g., `max_tokens = 512`).
- **Colab Errors**:
  - If dependencies fail to install, rerun the `!pip install` cell.
  - For large files, adjust the chunk size to avoid exceeding the model’s token limits.
  - If summarization fails for a chunk, the notebook will log the error and continue with the next chunk.
- **General**:
  - Refer to [OpenRouter Documentation](https://openrouter.ai/docs/quickstart) for API details.
  - Contact OpenRouter support if you face persistent API-related issues.

By following these steps, you should be able to set up and run the summarizer notebook successfully. For further details, see the [README.md](README.md).