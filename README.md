# wikiHow-FG-Corpus

This repository contains the wikiHow flow graph (wikiHow-FG) corpus, flow graph annotations of 120 articles in four domains. More information is provided in our paper, [Towards Flow Graph Prediction of Open-Domain Procedural Texts](https://arxiv.org/abs/2305.19497).

## Data Structure
The `data` directory contains four directories for annotated articles of each domain. The annotated articles are provided as json files. Each json file contains:

- `steps`: A list of steps, and each step contains a list of tokens consisting of a token ID, word, and named entity tag. A token ID is represented in the form (step index)-(sentence index)-(word index).
- `flows`: A list of labeled edges. Each edge is a tuple of (i) the token ID of the start node, (ii) the token ID of the end node, and (iii) a label.
- `url`: A URL of the article.
- `article_id`: An article id used in [the wikiHow corpus](https://github.com/zharry29/wikihow-goal-step).

## Citation

```
@inproceedings{shirai2023towards,
    title = "Towards Flow Graph Prediction of Open-Domain Procedural Texts",
    author = "Shirai, Keisuke  and Kameko, Hirotaka  and Mori, Shinsuke",
    booktitle = "Proceedings of the 8th Workshop on Representation Learning for NLP (RepL4NLP 2023)",
    year = "2023",
    publisher = "Association for Computational Linguistics",
    pages = "87--96",
}

```


