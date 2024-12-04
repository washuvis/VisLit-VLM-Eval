# VLM Visualization Literacy Assessment

This repository contains the implementation and evaluation framework for assessing visualization literacy capabilities of Visual Language Models (VLMs) using standardized tests VLAT and CALVI. The study provides a comprehensive comparison of four state-of-the-art VLMs' abilities to interpret, reason about, and critically analyze data visualizations.

## 🎯 Project Overview

The project evaluates VLMs through:
- Visualization Literacy Assessment Test (VLAT) - 53 multiple-choice items across 12 visualization types
- Critical thinking Assessment for Literacy in Visualization (CALVI) - 45 items focused on misleading visualization elements
- 10 randomized evaluation runs per model to ensure robust results

## 🤖 Models Evaluated

| Model | Version | Provider |
|-------|----------|----------|
| GPT-4 Vision | GPT-4o | OpenAI |
| Claude | 3.5 Sonnet | Anthropic |
| Gemini | 1.5 Pro | Google |
| Llama | 3.2-vision | Meta |

All models are configured with:
- Temperature: 0
- Max tokens: 300

## 📁 Repository Structure

```
├── README.md
├── data/
│   ├── VLAT/                 # VLAT test images and questions
│   └── CALVI/                # CALVI test images and questions
├── scripts/
│   ├── gpt4_evaluation.ipynb        # GPT-4 Vision evaluation notebook
│   ├── claude_evaluation.ipynb      # Claude evaluation notebook
│   ├── gemini_evaluation.ipynb      # Gemini evaluation notebook
│   ├── llama_evaluation.ipynb       # Llama evaluation notebook
├── prompts/
│   ├── VLAT_prompt.txt      # Standardized VLAT assessment prompt
│   └── CALVI_prompt.txt     # Standardized CALVI assessment prompt
├── Output/
│   ├── CALVI/               # model responses to CALVI questions
│   ├── VLAT/                # model responses to VLAT questions
```

## 🚀 Getting Started

1. Clone the repository:
```bash
git clone https://github.com/washuvis/VisLit-VLM-Eval.git
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

3. Configure API keys:
   - Add your API keys for each VLM provider

4. Run evaluations:
   - Navigate to the `scripts` directory
   - Execute evaluation notebooks for each model

## 📧 Contact

For questions or feedback, please contact Saugat Pandey (p.saugat@wustl.edu) or Dr. Alvitta Ottley (alvitta@wustl.edu)