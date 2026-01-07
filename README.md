# Vietnamese Depression Level Classification using Large Language Models

## Project Overview

This project focuses on **classifying depression severity levels from Vietnamese narrative texts**
using a **Large Language Model (LLM)**.
The system is designed not only to predict a depression label but also to **generate
human-readable explanations** for its predictions.

The project is intended for **academic research and educational purposes**, particularly
in the fields of **Natural Language Processing (NLP)** and **mental health–related text analysis**.

---

## Task Definition

Given a Vietnamese free-form narrative text describing personal experiences,
emotions, or life events, the model assigns **exactly one depression level**
based on predefined guidelines.

The task is formulated as an **instruction-following text generation problem**,
where the model learns to follow detailed instructions and output a single label.

---

## Depression Levels

The system classifies texts into four levels:

- **1-Bình thường**  
  No or minimal depressive symptoms, stable emotional and functional state.

- **2-Nhẹ**  
  Mild emotional distress or anxiety with limited impact on daily life.

- **3-Vừa**  
  Moderate depression with noticeable effects on mental health and daily functioning.

- **4-Nặng**  
  Severe psychological distress, hopelessness, or emotional collapse.

These definitions are explicitly encoded in the instruction prompt to ensure
consistent interpretation during both training and inference.

---

## Methodology

The approach is based on the following principles:

- Treat depression classification as an **instruction-following task**
- Fine-tune a Vietnamese-capable LLM using **parameter-efficient adaptation**
- Preserve the original narrative structure and emotional flow of the text
- Encourage the model to reason over emotional cues and severity indicators

Rather than relying on surface-level keywords, the model learns to associate
narrative patterns, emotional expressions, and lived experiences with
corresponding depression levels.

---

## Explainable Prediction

In addition to label prediction, the system generates **natural language explanations**
describing why a particular label was chosen.

Explanations typically reference:

- Emotional states expressed in the narrative
- Repeated stressors or negative life events
- Indicators of psychological burden or resilience

This explainability component aims to improve **transparency and interpretability**,
which are essential for mental health–related applications.

---

## Data Characteristics

The dataset consists of Vietnamese narrative texts with highly variable lengths,
often containing long and detailed personal stories rather than short sentences.

Special attention is given to:

- Handling long-form narratives
- Preserving contextual coherence
- Addressing class imbalance across depression levels

These characteristics reflect real-world advice-seeking or counseling-style texts.

---

## Intended Use

This project is intended for:

- Academic research
- Educational demonstrations of LLM-based text classification
- Exploratory studies on explainable AI for mental health text analysis

**This system is not intended for clinical diagnosis or medical decision-making.**

---

## Ethical Considerations

All predictions produced by this system should be interpreted with caution.
The model does not replace professional mental health assessment and should be used
only for research or educational purposes.

---

## Future Directions

Potential extensions of this work include:

- Chunk-based or hierarchical reasoning for very long texts
- Improved faithfulness and diversity of explanations
- Multi-stage depression severity modeling
- Comparative analysis with traditional machine learning approaches
