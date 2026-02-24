# A-Comprehensive-and-Explainable-Evaluation-of-Embedding-Strategies-and-LLM-s-for-COVID-19-FND

# This research paper has been submitted to conferences and is currently under review.

## A Comprehensive and Explainable Evaluation of Large Language Models for COVID-19 Fake News Detection

This project presents an in-depth study on the use of Large Language Models (LLMs) for detecting COVID-19 fake news, with a strong emphasis on Explainable Artificial Intelligence (XAI) to understand and interpret model decisions.

The research focuses on moving beyond traditional black-box classification systems by incorporating reasoning-driven models and explainability techniques to improve trust, transparency, and reliability in high-stakes domains like healthcare.

## Overview

Fake news in the healthcare domain can have serious real-world consequences, influencing public behavior and policy decisions. While modern LLMs demonstrate strong performance in understanding and analyzing textual data, their lack of transparency poses a challenge for real-world deployment.

This work addresses that gap by combining:
- The reasoning capabilities of Large Language Models  
- The interpretability provided by Explainable AI techniques  

The goal is not only to achieve high detection performance but also to understand *why* a model makes a particular prediction.

## Large Language Models (LLMs)

This research explores the use of lightweight and efficient Large Language Models for fake news detection. Unlike traditional models that rely on pattern recognition, LLMs perform **reasoning-based classification** by analyzing the overall narrative, context, and semantic consistency of the input text.

Key aspects of LLM-based detection in this work include:

- **Instruction-based classification:**  
  Models are prompted to classify news as *Fake* or *Real* based on the given content.

- **Context-aware reasoning:**  
  Instead of focusing on individual words, LLMs evaluate the entire text to determine plausibility and coherence.

- **Zero-shot capability:**  
  LLMs can perform classification without task-specific training, making them adaptable to emerging misinformation.

- **Semantic and narrative understanding:**  
  The models detect subtle inconsistencies, misleading claims, and unrealistic narratives that are difficult for traditional systems to capture.

This approach enables robust detection of complex and context-dependent fake news.

## Explainable Artificial Intelligence (XAI)

A major contribution of this work is the integration of explainability into LLM-based fake news detection.

Since LLMs are inherently black-box models, traditional feature attribution methods are not directly applicable. Therefore, this research adopts **behavior-based explainability techniques**, focusing on how models generate reasoning.

### Prompt-Based Rationale Generation

The primary explainability method used in this work is **prompt-based rationale generation**, where the model is instructed to output both:
- A classification label (Fake/Real)  
- A corresponding explanation for its decision  

This approach provides insights into:
- The reasoning process followed by the model  
- Key factors influencing the prediction  
- How the model interprets semantic meaning and context  

### Explanation Characteristics

The generated explanations typically highlight:

- **Narrative consistency:** Whether the story logically makes sense  
- **Factual plausibility:** Alignment with known real-world information  
- **Semantic coherence:** Consistency in claims and statements  
- **Misinformation cues:** Indicators of exaggeration, ambiguity, or manipulation  

### Interpretability vs Faithfulness

While prompt-based explanations provide valuable insights, this work also acknowledges that:
- These explanations reflect the model’s generated reasoning  
- They may not always perfectly represent internal computations  

Despite this limitation, they serve as an effective tool for understanding LLM behavior in practical scenarios.

## Key Contributions

- Application of Large Language Models for reasoning-based fake news detection  
- Integration of explainable AI techniques specifically tailored for LLMs  
- Detailed analysis of how LLMs interpret and evaluate misinformation  
- Demonstration of improved transparency in model decision-making  
- Focus on trust and reliability in healthcare-related AI systems  

## Conclusion

This work demonstrates that Large Language Models can effectively detect fake news by leveraging deep semantic understanding and reasoning capabilities. By incorporating explainability through prompt-based rationale generation, the study enhances transparency and builds trust in AI-driven systems.

The research highlights the importance of combining performance with interpretability, especially in sensitive domains like healthcare, where understanding model decisions is as critical as accuracy.

---

📄 For complete details, refer to the full research paper included in this repository.
