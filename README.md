\section*{Vietnamese Depression Level Classification using Large Language Models}

\subsection*{Project Overview}

This project focuses on the task of \textbf{classifying depression severity levels}
from \textbf{Vietnamese narrative texts} using a \textbf{Large Language Model (LLM)}.
The system is designed to not only predict a depression level but also to
\textbf{generate human-readable explanations} for its decisions.

The project is developed in the context of academic research and is suitable for
graduation theses or exploratory studies in
\textit{Natural Language Processing (NLP)} and \textit{Mental Health Informatics}.

---

\subsection*{Task Definition}

Given a Vietnamese free-form narrative text describing personal experiences,
emotions, or life events, the model assigns exactly \textbf{one} depression level
based on predefined guidelines.

The task is formulated as an \textbf{instruction-following text generation problem},
where the model learns to follow detailed classification instructions and output
a single label.

---

\subsection*{Depression Levels}

The system classifies texts into four levels:

\begin{itemize}
    \item \textbf{1-Bình thường}: No or minimal depressive symptoms, stable functioning
    \item \textbf{2-Nhẹ}: Mild emotional distress or anxiety with limited impact
    \item \textbf{3-Vừa}: Moderate depression affecting daily life and mental stability
    \item \textbf{4-Nặng}: Severe psychological distress, hopelessness, or emotional collapse
\end{itemize}

These levels are defined through explicit instructions embedded in the prompt,
ensuring consistent interpretation during both training and inference.

---

\subsection*{Methodology}

The approach is based on the following key ideas:

\begin{itemize}
    \item Treat depression classification as an instruction-following task
    \item Fine-tune a Vietnamese-capable LLM using parameter-efficient techniques
    \item Preserve the original narrative style of the input text
    \item Encourage the model to reason about emotional cues and severity indicators
\end{itemize}

The model learns to associate narrative patterns, emotional expressions, and
life circumstances with corresponding depression levels.

---

\subsection*{Explainable Prediction}

Beyond label prediction, the system is designed to produce
\textbf{natural language explanations} describing why a particular label was chosen.

Explanations typically reference:
\begin{itemize}
    \item Emotional states expressed in the text
    \item Repeated negative experiences or stressors
    \item Indicators of psychological burden or resilience
\end{itemize}

This explainability component aims to improve transparency and interpretability,
which are critical for mental health–related applications.

---

\subsection*{Data Characteristics}

The dataset consists of Vietnamese narrative texts with varying lengths,
often containing long personal stories rather than short sentences.
This reflects real-world scenarios such as counseling submissions or advice-seeking posts.

Special attention is given to:
\begin{itemize}
    \item Handling long and detailed narratives
    \item Preserving contextual coherence
    \item Addressing class imbalance across depression levels
\end{itemize}

---

\subsection*{Intended Use}

This project is intended for:
\begin{itemize}
    \item Academic research
    \item Educational demonstrations of LLM-based text classification
    \item Exploratory analysis of explainable AI in mental health
\end{itemize}

\textbf{It is not intended for clinical diagnosis or medical decision-making.}

---

\subsection*{Ethical Considerations}

Depression level predictions produced by this system do not constitute a medical diagnosis.
All outputs should be interpreted with caution and used only for research or educational purposes.

---

\subsection*{Future Directions}

Potential extensions of this work include:
\begin{itemize}
    \item Chunk-based reasoning for very long texts
    \item Improved explanation faithfulness
    \item Multi-stage or hierarchical severity classification
    \item Comparative studies with traditional machine learning models
\end{itemize}
