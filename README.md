# RankAI – MVP

RankAI is a task-specific, constraint-aware AI benchmarking system that evaluates and ranks AI models based on measurable performance metrics rather than opinions.

This MVP focuses on **text summarization** and compares multiple open-source transformer models using:
- Accuracy (ROUGE)
- Latency
- Hallucination-aware proxies

---

## 🚀 Why RankAI?
Most AI comparisons answer: *“Which model is best?”*

RankAI answers:
> **“Which AI model is best for this task under these constraints?”**

This mirrors how real companies select models for production.

---

## 🧠 How It Works
1. Load a benchmark dataset with ground truth summaries
2. Run the same task across multiple AI models
3. Measure accuracy, latency, and hallucination risk
4. Apply directional adjustment and weighted scoring
5. Produce an explainable ranking

---

## 📊 Metrics Used
- **ROUGE-1** for summarization accuracy
- **Inference latency** as a performance metric
- **Output-length proxy** for hallucination risk
- **Weighted final score** for ranking decisions

---

## 🤖 Models Evaluated
- T5-small
- DistilBART-CNN
- Pegasus (ArXiv)

All models are open-source and evaluated offline (no paid APIs).

---

## 🛠 Tech Stack
- Python
- Hugging Face Transformers
- Hugging Face Datasets
- ROUGE Score
- Pandas / NumPy

---

## 📌 Future Improvements
- Replace proxies with factual consistency checks
- Add user-defined metric weights
- Support real-time API-based models (GPT, Claude, Gemini)
- Build a lightweight dashboard

---

## 👤 Author
Built as an MVP to demonstrate industry-style AI evaluation and decision-making.
