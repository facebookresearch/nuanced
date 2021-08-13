# NUANCED: Natural Utterance Annotation for Nuanced Conversation with Estimated Distributions

## Dataset Overview

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

## Citations

If you want to publish experimental results with our datasets or use the baseline models, please cite the following articles:
```
@article{chen2020nuanced,
  title={NUANCED: Natural Utterance Annotation for Nuanced Conversation with Estimated Distributions},
  author={Chen, Zhiyu and Liu, Honglei and Xu, Hu and Moon, Seungwhan and Zhou, Hao and Liu, Bing},
  journal={arXiv preprint arXiv:2010.12758},
  year={2020}
}
```
```
@inproceedings{xu2020user,
  title={User Memory Reasoning for Conversational Recommendation},
  author={Xu, Hu and Moon, Seungwhan and Liu, Honglei and Liu, Bing and Shah, Pararth and Philip, S Yu},
  booktitle={Proceedings of the 28th International Conference on Computational Linguistics},
  pages={5288--5308},
  year={2020}
}
```

## License

NUANCED is released under [CC-BY-NC-4.0](https://creativecommons.org/licenses/by-nc/4.0/), see [LICENSE](LICENSE) for details.
