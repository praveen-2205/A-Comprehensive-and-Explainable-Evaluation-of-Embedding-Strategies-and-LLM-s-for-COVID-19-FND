# This research paper has been submitted to conferences and is currently under review.

## Explainable Fake News Detection using Large Language Models (LLMs)

This project presents a comprehensive approach to fake news detection in the COVID-19 domain using **Large Language Models (LLMs)**, combined with **Explainable Artificial Intelligence (XAI)** techniques to ensure transparency and interpretability of model decisions.

The primary objective is to move beyond black-box predictions and provide **reasoning-driven, explainable outputs** for high-stakes applications such as healthcare misinformation detection.

---

## 🔹 Large Language Models (LLMs)

This work leverages modern LLMs to perform **reasoning-based classification**, where the model evaluates the entire text context instead of relying on surface-level patterns.

### Models Used

- **LLaMA 2 (7B)**
  - High-performance LLM with strong contextual understanding
  - Capable of reasoning over long textual inputs
  - Achieved the highest accuracy (~97.8%) in experiments

- **Qwen 7B-Instruct**
  - Instruction-tuned LLM designed for prompt-based tasks
  - Effective in zero-shot classification scenarios
  - Generates structured and interpretable outputs

---

### LLM Approach

The models are used in a **zero-shot setting**, meaning:
- No task-specific fine-tuning is performed
- Models rely purely on **prompt-based reasoning**

Each input is processed using:
- **Instruction-based prompting**
- **Context-aware reasoning**
- **Narrative and semantic analysis**

Instead of focusing on keywords, the models evaluate:
- Logical consistency of the content  
- Plausibility of claims  
- Alignment with real-world knowledge  

This enables detection of **subtle and context-dependent misinformation**.

---

## 🔹 Explainable Artificial Intelligence (XAI)

A major contribution of this work is the integration of multiple XAI techniques to analyze and interpret model behavior across different paradigms.

The approach combines:
- **Feature-based explainability (LIME, SHAP)**
- **Reasoning-based explainability (LLMs)**

---

## 🔹 XAI Methods Used

### 1. LIME (Local Interpretable Model-agnostic Explanations)

LIME is used to provide **local interpretability** for individual predictions.

#### How it works:
- The input text is perturbed (slightly modified)
- The model's predictions on these variations are observed
- Important words influencing the prediction are identified

#### What it provides:
- Word-level importance for a specific prediction  
- Identification of tokens pushing classification toward *Fake* or *Real*  
- Easy-to-understand local explanations  

---

### 2. SHAP (SHapley Additive exPlanations)

SHAP is based on **game theory** and provides both **local and global interpretability**.

#### How it works:
- Each feature (word/token) is assigned a contribution score
- Scores represent the impact of that feature on the final prediction

#### What it provides:
- Consistent feature attribution  
- Global understanding of model behavior  
- Positive/negative contribution of words  

---

### 3. Prompt-Based Rationale Generation (LLM-Based XAI)

This is the **primary explainability technique for LLMs**.

#### Approach:
The model is prompted to generate:
- A classification label (*Fake / Real*)  
- A natural language explanation supporting its decision  

#### Example Output:
