NUANCED dataset

- Folder data_dist: the nuanced version;
- Folder data_discrete: the coarse version with 0-1 labels;
- meta.json: ontology for this restaurant domain;


Format for the dataset:
A list of dictionarys, with each dictionary as one dialogue of the following important fields:
    "dialogue": a list of dialog turns. Each turn has the following fields:
        "role": user or assistant
        "text": user utterance or system response
        "dialog_acts": acts of this turn
        "slots": slots involved in this turn
        "dist": for user turn, the preference distribution
        "strategy": strategy 1 means the user utterance does not have grounded ontology terms (implicit reasoning), strategy 2 means the user utterance has grounded ontology terms
