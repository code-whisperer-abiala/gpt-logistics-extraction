
# From Shipping Logs to Smart Extraction: Fine-Tuning GPT-3.5 for Logistics Tasks

This project demonstrates how to fine-tune GPT-3.5 to extract structured fields like invoice numbers, PO references, delivery dates, and costs from messy, human-written logistics messages.

## Project Type
NLP / Fine-Tuning / Prompt Engineering

## Tools & Tech
- OpenAI API (fine-tuning endpoint)
- Python (Google Colab)
- JSONL-formatted training data
- Matplotlib for training curves

## Goal
To build a model that extracts structured values (e.g., PO numbers, invoice totals) from unstructured logistics text, reducing human intervention and parsing errors in real operations.

---

## File Structure

- `notebook/` — Google Colab notebook for model training, evaluation, and testing
- `data/` — Cleaned `.jsonl` training and validation datasets
- `visuals/` — Model loss curve + evaluation summary image
- `README.md` — Project overview and usage
- `requirements.txt` — Python packages (if applicable)

---

## Model Training Summary

| Epoch | Validation Loss |
|-------|-----------------|
| 5     | ~1.02           |
| 3     | ~0.83           |
| **2** (final) | **~0.01**    |

Final evaluation accuracy: **52.63%** on 19 mixed-format test prompts.

---

## Visuals

### Loss Curve
![Training Curve](visuals/training_curve.png)

### Model Evaluation
![Evaluation Table](visuals/evaluation_table.png)

---

## How to Run (Basic Guide)
1. Upload your `.jsonl` files to Google Colab.
2. Install OpenAI with `!pip install openai`
3. Use the notebook to fine-tune and evaluate the model.

---

## Use Cases
- Extracting PO #s from scanned delivery emails
- Parsing invoice totals for backend reporting
- Building GPT-based logistic chatbots or form auto-filling

---

## 👤 Author
**Grace Isiaka**  
[Portfolio on Notion](https://www.notion.so/Grace-Isiaka-Data-Analytics-Portfolio-1e0ace9f2e3a8043bf78e72b72b603c3) | [LinkedIn](https://www.linkedin.com/in/grace-isiaka-97002aa8/)

---

## If you liked this project...
- Give it a ⭐️ on GitHub
- Follow for more projects where data meets applied AI
