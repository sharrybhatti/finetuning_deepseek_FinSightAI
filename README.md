

# 🧠 Finetuned DeepSeek Finance

A fine-tuned version of [DeepSeek LLM 7B](https://huggingface.co/deepseek-ai/deepseek-llm-7b) on financial documents and balance sheet Q&A using PEFT (LoRA). This model is optimized for financial text generation, report summarization, and corporate finance analysis.

---

## 🚀 Features

- 💹 Trained on balance sheets and financial Q&A
- ⚙️ Based on DeepSeek 7B architecture
- 📦 Fine-tuned using PEFT (LoRA) for efficient parameter updates
- 📊 Suitable for financial summarization, forecasting prompts, and analytical assistants

---

## 🛠️ Installation

```bash
pip install transformers accelerate peft

    Make sure you have a GPU-enabled environment with at least 16GB of VRAM.

🔧 Usage

from transformers import pipeline

pipe = pipeline(
    "text-generation",
    model="sharybhatti/finetuned-deepseek-finance",
    trust_remote_code=True
)

prompt = "Summarize the Q4 2023 balance sheet for Company XYZ:"
response = pipe(prompt, max_new_tokens=200)
print(response[0]["generated_text"])


📈 Evaluation Metrics
Metric	Score
BLEU	0.0576
ROUGE-1	0.2303
ROUGE-2	0.1226
ROUGE-L	0.1938
BERTScore F1	0.8559

📚 Model Details

    Base Model: deepseek-ai/deepseek-llm-7b

    Fine-tuning Method: LoRA (via PEFT v0.15.2)

    Languages: English

    Training Duration: ~8 GPU hours (A100)

    Dataset: Financial documents, corporate balance sheets, and QA pairs

📦 Model on Hugging Face

🔗 View on Hugging Face sharybhatti/finetuned-deepseek-finance
🛑 Limitations

    Not intended for use as a sole decision-maker in financial advice or investments.

    May hallucinate values or interpret data incorrectly if not prompted properly.

📄 License

Apache 2.0 – free for commercial and research use.
👨‍💻 Author

Shaharyar Bhatti
GitHub • sharry.bhatti1@gmail.com

    Built with ❤️ for financial intelligence tools & research.


---
