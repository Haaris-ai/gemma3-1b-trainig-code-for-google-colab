# 🚀 Gemma 3 Training for Google Colab

This repository provides a streamlined workflow for fine-tuning Google's **Gemma 3** models using Google Colab and the Unsloth library for 2x faster training.

---

## 📋 Prerequisites

* **Dataset:** You must have a training dataset (recommended to make with ai **specify Gemma**)**named `dataset.jsonl`** to upload to notebook.
* **Hugging Face Account:** Required to access the model weights.
* **Hardware:** This notebook is optimized for a **T4 GPU** (available on the free tier of Colab).

---

## 🛠️ Setup Instructions

### 1. Access the Model
1. Sign up or log in at [Hugging Face](https://huggingface.co).
2. Visit the [Gemma 3 4B-it Model Page](https://huggingface.co/google/gemma-3-4b-it).
3. Accept the license agreement. *Note: Accessing one Gemma 3 model usually grants access to the entire family.*

### 2. Create a Hugging Face Token
1. Click your profile icon (top right) and go to **Settings** > **Access Tokens**.
2. Click **Create new token** and name it `colab_gemma`.
3. Copy the token immediately; you will need it for the next step.

### 3. Configure Google Colab
1. Open [Google Colab](http://colab.research.google.com).
2. Go to **File** > **Upload notebook** and select the specific for your Gemma 3 model`.ipynb` file from this repo.
3. On the left sidebar, click the **Folder icon (Files)**
4. Upload your **dataset.jsonl** file in root
5. On the left sidebar, click the **Key icon (Secrets)**.
6. Add a new secret:
   * **Name:** `HF_TOKEN`
   * **Value:** Paste your Hugging Face access token.
   * **Permission:** Toggle "Notebook access" to **On**.

---

## 🚄 Training Execution

1. **Set Runtime:** Click the arrow next to the **Runtime** button (top right) > **Change runtime type**. Select **T4 GPU** and click Save.
2. **Upload Dataset:** * Ensure your file is named `dataset.jsonl`.
   * Click the **Folder icon** on the left sidebar and upload the file.
3. **Run All:** Click **Runtime** > **Run all** (or `Ctrl + F9`).
4. The **ollama .gguf** file will be in your google drve

---

### 💡 Pro-Tips
* **Dataset Format:** Ensure your `.jsonl` entries match the Gemma 3 prompt template for the best results.
* **Saving:** Your fine-tuned model will be saved in the `/outputs` folder within the Colab file browser.

---
