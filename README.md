# Causal Learning From Textual Data

This project focuses on causal learning from textual data, where the input consists of pairs of texts, and the task is to determine if a causal relationship exists between them. The process is structured into four key stages. First, the model identifies correlations between variables, analyzing if textual features suggest a connection. Second, a causal skeleton is built, representing the potential relationships without considering their direction. Third, the model assesses causal directionality, distinguishing cause from effect within the identified skeleton. Finally, we evaluate the model's reasoning and explainability, ensuring that it can not only uncover causal patterns but also provide transparent, interpretable explanations for its predictions.

We are particularly interested in exploring causal relationships between complex events that are domain-specific, moving beyond simple patterns commonly identified by conjunctions like because, due to, as a consequence of, and others. These simplistic linguistic cues may capture basic cause-and-effect interactions, but they often fail to represent the nuanced, context-dependent relationships between complex events that arise in real-world scenarios.

# Datasets

## HeadlineCause: A Dataset of News Headlines for Detecting Causalities

_Description_: the first headline causes the second headline if the second headline is impossible without the first one. If the first event did not happen, then the second event must not be happening too.

- **Paper**: [https://arxiv.org/pdf/2108.12626](https://arxiv.org/pdf/2108.12626)
- **Download**: [https://github.com/IlyaGusev/HeadlineCause/releases/tag/v1.0](https://github.com/IlyaGusev/HeadlineCause/releases/tag/v1.0)

An example of a news headline pair with a causal relation (sample en_tg_1153):

- A: Oklahoma spent $2 million on malaria drug touted by Trump  
- B: Gov. Kevin Stitt defends $2 million purchase of malaria drug touted by Trump

## Risk management and situation awareness

_Description_: target application is risk management and situation awareness, where the “causal” knowledge can help analysts and decision makers better understand the impact of past and current events and conditions on relevant outcomes. A key requirement in this application is the ability to support causes (Xs) and effects (Ys) that are general phrases, without any semantic constraints.

- **Paper**: [https://www.ijcai.org/proceedings/2019/695](https://www.ijcai.org/proceedings/2019/695)
- **Download**: [https://github.com/GoloMarcos/eCOLGAT/blob/main/datasets/risk-models-benchmark-v1.csv](https://github.com/GoloMarcos/eCOLGAT/blob/main/datasets/risk-models-benchmark-v1.csv)


Examples: 

| Cause                                            | Effect                                                       |
|--------------------------------------------------|---------------------------------------------------------------|
| Currency appreciation against US dollar          | Low inflation                                                 |
| Decreased local protectionism                    | Decreased tariffs on foreign firms                            |
| Decreasing government and political stability    | Decrease in government spending (infrastructure, education, public benefits) |
| OPEC's agreement to raise production quota       | Low oil prices                                                |
| Expansionary fiscal policy                       | Increased government spending                                 |



### FinCausal Shared Task: Financial Document Causality Detection

_Description_: This task focuses on determining causality associated with a quantified fact. An event is defined as the arising or emergence of a new object or context regarding a previous situation. So, the task will emphasize the detection of causality associated with the transformation of financial objects embedded in quantified facts. The aim is to identify, in a causal sentence or text block, the causal elements and the consequential ones.

- **Shared Task**: [https://codalab.lisn.upsaclay.fr/competitions/14596](https://codalab.lisn.upsaclay.fr/competitions/14596)
- **Download (2022)**: [https://github.com/yseop/YseopLab/blob/develop/FNP_2022_FinCausal/data/practice_addition_fnp2022-fincausal-task2.csv](https://github.com/yseop/YseopLab/blob/develop/FNP_2022_FinCausal/data/practice_addition_fnp2022-fincausal-task2.csv)

Examples:

| **Text** | **Cause** | **Effect** |
|----------|-----------|------------|
| Boussard Gavaudan Investment Management LLP bought a new position in shares of GENFIT S A/ADR in the second quarter worth about $199,000. Morgan Stanley increased its stake in shares of GENFIT S A/ADR by 24.4% in the second quarter. Morgan Stanley now owns 10,700 shares of the company’s stock worth $211,000 after purchasing an additional 2,100 shares during the period | Morgan Stanley increased its stake in shares of GENFIT S A/ADR by 24.4% in the second quarter | Morgan Stanley now owns 10,700 shares of the company’s stock worth $211,000 after purchasing an additional 2,100 shares during the period |
| Zhao found himself 60 million yuan indebted after losing 9,000 BTC in a single day (February 10, 2014) | losing 9,000 BTC in a single day (February 10, 2014) | Zhao found himself 60 million yuan indebted |
