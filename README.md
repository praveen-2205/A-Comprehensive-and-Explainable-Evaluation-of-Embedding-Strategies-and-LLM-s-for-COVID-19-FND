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
Label: Fake
Reason: The claim lacks scientific evidence and uses exaggerated language...

#### What it provides:
- Human-readable explanations  
- Insight into model reasoning  
- Context-aware interpretation  

---

### 4. Semantic and Narrative-Level Analysis

Unlike traditional XAI methods, LLM explanations operate at a higher level.

#### Focus:
- Overall meaning of the text  
- Flow and consistency of the narrative  
- Relationships between different parts of the content  

#### Benefits:
- Detects subtle misinformation  
- Handles complex and nuanced text  

---

### 5. Factual Plausibility Reasoning

The model evaluates whether the claims in the text:
- Align with real-world knowledge  
- Are logically and scientifically valid  

#### Helps identify:
- False or misleading medical claims  
- Unrealistic or exaggerated information  

---

### 6. Qualitative Evaluation of Explanations

Generated explanations are evaluated based on:

- **Coherence** → Logical and understandable reasoning  
- **Relevance** → Directly related to the input text  
- **Consistency** → Aligns with the predicted label  

---

## ⚠️ Important Insight

- **LIME & SHAP** → Feature-based explainability (word-level importance)  
- **LLM-based XAI** → Reasoning-based explainability (semantic understanding)  

While LLM explanations provide strong interpretability, they are:
- Generated outputs (not direct internal attributions)  
- Hence, **interpretable but not fully faithful**

---

## 🔥 Key Contributions

- Use of **LLaMA 2 and Qwen LLMs** for reasoning-based fake news detection  
- Integration of **LIME and SHAP** for feature-level interpretability  
- Development of **prompt-based rationale generation** for LLM explainability  
- Combination of **feature-based and reasoning-based XAI techniques**  
- Focus on transparency and trust in healthcare AI systems  

---

## 📄 Note

Refer to the full research paper included in this repository for detailed experiments, results, and analysis.
