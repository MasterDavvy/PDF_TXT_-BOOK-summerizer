# OpenRouter API Key Setup Guide

This guide explains how to obtain and use an OpenRouter API key to run the PDF/TXT Summarizer notebook in Google Colab.

## Step 1: Sign Up for OpenRouter

1. Visit [OpenRouter.ai](https://openrouter.ai).
2. Click **Sign Up** or **Get Started** in the top-right corner.
3. Create an account using your email, Google, GitHub, or another supported authentication method.
4. Follow the prompts to complete the sign-up process and verify your email if required.

## Step 2: Generate an API Key

1. Log in to your OpenRouter account.
2. Navigate to your **Profile** or **Settings** (typically found by clicking your account name or icon).
3. Locate the **API Keys** section in the dashboard.
4. Click **Generate New Key** or a similar option to create a new API key.
5. Copy the API key to a secure location (e.g., a password manager or a temporary note). **Do not share this key publicly.**

## Step 3: Use the API Key in the Notebook

1. Open the `summarizer.ipynb` notebook in Google Colab (via the "Open in Colab" badge in [README.md](README.md) or by uploading it to your Google Drive).
2. Run the first cell to install dependencies.
3. When prompted with `🔑 OpenAI / OpenRouter key :`, paste your API key and press Enter.
4. Continue with the remaining prompts (e.g., model name, chunk size) to configure the summarizer.
   - The default model is `meta-llama/llama-4-maverick`. You can press Enter to use it or enter another model ID from [OpenRouter Models](https://openrouter.ai/models).

## Step 4: Verify Model Availability

- The notebook uses `meta-llama/llama-4-maverick` by default. Ensure this model (or any custom model you choose) is available by checking [OpenRouter Models](https://openrouter.ai/models).
- Some models may require credits or have specific token limits. Review the model details on OpenRouter to confirm compatibility.

## Troubleshooting

- **Invalid API Key**: Double-check that you copied the key correctly without extra spaces.
- **API Errors**: Ensure your OpenRouter account has sufficient credits (some models require paid credits). Check your account dashboard for details.
- **Model Issues**: If the selected model fails, verify its ID on [OpenRouter Models](https://openrouter.ai/models) and try another model if needed.
- **Need Help?**: Refer to [OpenRouter Documentation](https://openrouter.ai/docs/quickstart) or contact OpenRouter support.

By following these steps, you’ll have your OpenRouter API key ready to use with the summarizer notebook. For additional setup details, see [SETUP.md](SETUP.md).