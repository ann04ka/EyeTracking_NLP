# Eye Tracking + NLP: Automated Description of Gaze Trajectories

This project focuses on the automatic generation of textual descriptions of gaze trajectories based on eye-tracking visualizations using Vision-Language Models (VLMs).

## 🧩 Task Description

Eye tracking allows us to analyze where a person is looking, but interpreting the data requires time and expertise. We address the task of automatically translating visualized eye-tracking data (fixations, saccades, pupil changes) into structured natural language descriptions.

## 📁 Repository Contents

- `EyeTracking_NLP.ipynb` — Jupyter Notebook with code for model training and evaluation.
- `AnnotatingImages.ipynb` — Jupyter Notebook with code for creating annotations for eye-tracking images.

## 🤖 Models Used

We test and fine-tune the following Vision-Language models:
- **Qwen2.5-VL**
- **Gemma 3 4B**
- Classic Image-to-Text models: BLIP, GIT, ViT-GPT2, Paligemma

## 📊 Metrics

The quality of generated descriptions is evaluated using three metrics:
- **Total Similarity** — overall score combining semantics and answer accuracy.
- **Semantic Similarity** — similarity to the reference description (based on Sentence-BERT).
- **Answer Accuracy** — accuracy in recognizing the user's final choice.

## ✅ Requirements

To run the notebooks, install the following dependencies:

```bash
pip install transformers datasets accelerate sentence-transformers
```

## 📚 Acknowledgments

- [Qwen-VL](https://github.com/QwenLM/Qwen-VL)   
- [Gemma](https://deepmind.google/technologies/gemma/)   
- [Sentence-BERT](https://www.sbert.net/)   

## 📎 Additional Materials

- [Project Paper (PDF)](NLP_EyTracking.pdf) — detailed description of the task, methods, and research results.
