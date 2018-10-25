# Datasets Proximity Mining with OpenML

This page is dedicated for the Data Governance in Data Lakes project by the [DTIM Research Group](http://www.essi.upc.edu/dtim), UPC. We provide here the main datasets and sources for experimental evaluation of our techniques on [OpenML](https://www.openml.org) data.

## Getting Started

We provide the annotated ground-truth used in our experiments under the folder "datasets". There are two main types of files there provided in the Comma Separated Values (CSV) format:

* The "index" CSV files: They store the original index of datasets collected for the training set or the testing set in the experiments. It comes with the OpenML dataset ID, the dataset name, and the meta-features collected for each dataset.
* The "matching" CSV files: They store the meta-features' distances between all pairs of datasets in the training set or the testing set of the experiments. It comes with the OpenML dataset ID, the dataset name, the meta-features distances between the pair in each row, and the ground-truth of the relationships between the datasets in the pair: datesets_subject_main_match (1 or 0) for the Rel(d1,d2) relationship and datesets_duplicates_match (1 or 0) for the Dup(d1,d2) relationship.


To retrieve the original datasets from OpenML using the APIs provided by them and the dataset IDs (did) from our CSV files, please refer to the [OpenML API guide](https://www.openml.org/guide).


## Built With

* [Java OpenML API](https://www.openml.org/guide#!java)
* [Postgres DB](https://www.postgresql.org/)
* [WEKA Machine Learning Environment](http://www.cs.waikato.ac.nz/ml/weka/)
* [Apache Lucene](http://lucene.apache.org/)

## License

This project is licensed under the Apache License 2.0 License - see the [LICENSE.md](LICENSE) file for details.

## Acknowledgments
We are sincerely thankful to all the annototators who have validated and collaborated in creating the ground-truth datasets for the experiments. We thank the collaborators from the school of Pharmacy for helping us with the annotation of the datasets.

## Reference
For more details about the datasets in this project, how they were collected, and for a detailed description of the data collected, please see the main publication resulting from this project: _"Alserafi, A., Calders, T., Abelló, A., & Romero, O. (2017, October). **DS-Prox: Dataset Proximity Mining for Governing the Data Lake.** In International Conference on Similarity Search and Applications (pp. 284-299). Springer, Cham."_.
