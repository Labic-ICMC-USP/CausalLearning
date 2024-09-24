# Causal Learning From Textual Data

This project focuses on causal learning from textual data, where the input consists of pairs of texts, and the task is to determine if a causal relationship exists between them. The process is structured into four key stages. First, the model identifies correlations between variables, analyzing if textual features suggest a connection. Second, a causal skeleton is built, representing the potential relationships without considering their direction. Third, the model assesses causal directionality, distinguishing cause from effect within the identified skeleton. Finally, we evaluate the model's reasoning and explainability, ensuring that it can not only uncover causal patterns but also provide transparent, interpretable explanations for its predictions.

# Datasets

## HeadlineCause: A Dataset of News Headlines for Detecting Causalities

- **Paper**: [https://arxiv.org/pdf/2108.12626](https://arxiv.org/pdf/2108.12626)
- **Download**: [https://github.com/IlyaGusev/HeadlineCause/releases/tag/v1.0](https://github.com/IlyaGusev/HeadlineCause/releases/tag/v1.0)

_Description_: the first headline causes the second headline if the second headline is impossible without the first one. If the first event did not happen, then the second event must not be happening too.

An example of a news headline pair with a causal relation (sample en_tg_1153):

- A: Oklahoma spent $2 million on malaria drug touted by Trump  
- B: Gov. Kevin Stitt defends $2 million purchase of malaria drug touted by Trump
