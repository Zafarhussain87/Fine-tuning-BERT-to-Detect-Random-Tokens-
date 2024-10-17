# Training a Language Model to Learn the Syntax of Commands

To protect systems from malicious activities, it is important to differentiate
between valid and harmful commands. One way to achieve this is by learning
the syntax of the commands, which is a complex task because of the expansive
and evolving nature of command syntax. To address this, we harnessed
the power of a language model. Our methodology involved constructing a
specialized vocabulary from our commands dataset, and training a custom
tokenizer with a Masked Language Model head, resulting in the development
of a BERT-like language model. This model exhibits proficiency in learning
command syntax by predicting masked tokens. In comparative analyses, our
language model outperformed the Markov Model in categorizing commands
using clustering algorithms (DBSCAN, HDBSCAN, OPTICS). The language
model achieved higher Silhouette scores (0.72, 0.88, 0.85) compared to the
Markov Model (0.53, 0.25, 0.06) and demonstrated significantly lower noise
levels (2.63%, 5.39%, 8.49%) versus the Markov Model’s higher noise rates
(9.31%, 29.85%, 50.35%). Further validation with manually crafted syntax
and BERTScore assessments consistently produced metrics above 0.90 for
precision, recall, and F1-score. Our language model excels at learning command
syntax, enhancing protective measures against malicious activities.

# Cite as:
Hussain, Z., Nurminen, J. K. & Ranta-aho, P. “Training a language model to learn the syntax of commands” 2024, In: Array. 23, 100355.



