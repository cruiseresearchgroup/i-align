# i-Align: An Interpretable Knowledge Graph Alignment Model

i-Align is an interpretable knowledge graph alignment model that accurately predicts entity alignments between knowledge graphs and provides explanations for each prediction. The explanations are in the form of the most influential attributes and neighbors of the aligned entities, which can help experts decide the correctness of the alignment.

## Features

- **Accurate Entity Alignment**: i-Align achieves state-of-the-art performance in entity alignment tasks, accurately finding entities representing the same real-world entity across different knowledge graphs.

- **Interpretable Predictions**: Unlike existing methods, i-Align generates explanations for each alignment prediction in the form of the top-n most influential attributes and neighbors of the aligned entities.

- **Scalable**: i-Align can handle large knowledge graphs by using a novel Transformer-based Graph Encoder (Trans-GE) with Edge-gated Attention and Historical Embeddings.

## Installation

```bash
git clone https://github.com/cruiseresearchgroup/i-align.git
```

## Data Format

i-Align expects the following data files:

- `KG1_ENTITIES`: A pickle file containing the entities and their neighbors in the first knowledge graph.
- `KG2_ENTITIES`: A pickle file containing the entities and their neighbors in the second knowledge graph.
- `KG1_ATTRIBUTES`: A pickle file containing the entities and their attributes in the first knowledge graph.
- `KG2_ATTRIBUTES`: A pickle file containing the entities and their attributes in the second knowledge graph.
- `KG1_ent_vocab`, `KG2_ent_vocab`, `pred_vocab`, `char_vocab`: Pickle files containing vocabularies for entities, predicates, and characters.
- `seed_data`: A pickle file containing the seed alignment for training.
- `test_data`: A pickle file containing the test data for evaluation.

## Contributing

We welcome contributions to i-Align! Please submit a pull request or open an issue on the GitHub repository.

## Citation

If you use i-Align in your research, please cite the following paper:

```bibtex
@article{trisedya2023align,
  title={i-Align: an interpretable knowledge graph alignment model},
  author={Trisedya, Bayu Distiawan and Salim, Flora D and Chan, Jeffrey and Spina, Damiano and Scholer, Falk and Sanderson, Mark},
  journal={Data Mining and Knowledge Discovery},
  volume={37},
  number={6},
  pages={2494--2516},
  year={2023},
  publisher={Springer}
}
```

## Acknowledgments

This research is supported by the Australian Research Council (ARC) Centre of Excellence for Automated Decision-Making and Society (ARC CE200100005).
