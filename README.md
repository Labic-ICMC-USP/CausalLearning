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

## Risk management and situation awareness
- **Paper**: [https://www.ijcai.org/proceedings/2019/695](https://www.ijcai.org/proceedings/2019/695)
- **Download**: [https://github.com/GoloMarcos/eCOLGAT/blob/main/datasets/risk-models-benchmark-v1.csv](https://github.com/GoloMarcos/eCOLGAT/blob/main/datasets/risk-models-benchmark-v1.csv)

_Description_: target application is risk management and situation awareness, where the “causal” knowledge can help analysts and decision makers better understand the impact of past and current events and conditions on relevant outcomes. A key requirement in this application is the ability to support causes (Xs) and effects (Ys) that are general phrases, without any semantic constraints.

Examples: (cause -> effect)

- currency appreciation against US dollar -> low inflation
- decreased local protectionism -> decreased tariffs on foreign firms
- decreasing government and political stability -> decrease in government spending (infrastructure, education, public benefits)
- OPEC's agreement to raise production quota -> Low oil prices
- Expansionary fiscal policy -> increased government spending
