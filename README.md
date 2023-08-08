# GeoLingIt task 🗺 EVALITA2023 
This repository contains material for my first paper "Salogni at GeoLingIt: Geolocalization by Fine-tuning BERT", submitted in July 2023 for the 8th evaluation campaign [EVALITA 2023](https://www.evalita.it/campaigns/evalita-2023/).
By fine-tuning three Transformer models, two based on BERT ([AlBERTo](https://github.com/marcopoli/AlBERTo-it) and [bert-base-italian-cased](https://huggingface.co/dbmdz/bert-base-italian-cased)) and the other on RoBERTa ([umberto-commoncrawl-cased-v1](https://huggingface.co/Musixmatch/umberto-commoncrawl-cased-v1)), I aim at geolocating sequences exhibiting
non-standard Italian varieties relying solely on linguistic content.
I find that, given that the information contained in the embeddings is all we need to carry out this complex task, a model architecture with less task-specific layers leads to better results. 
Furthermore, in this project, the models pre-trained on miscellaneous corpora generalized better than those trained exclusively on tweets.
The work also shows that the greater availability of resources of a certain regional variety positively affects the capacity of
the model.

## Dataset 
[GeoLingIT](https://sites.google.com/view/geolingit) task data comprises 15K geotagged tweets that exhibit non-standard Italian language use (the content may be fully written in local language varieties or exhibiting code-switching with standard italian), and that have been collected in the corpus [DiatopIt](https://aclanthology.org/2023.vardial-1.19/). The data is annotated with latitude and longitude. Target and output coordinate data were normalized using Min-Max scaling

## Notebooks
* Reproducing the Analysis and Plots: [here](https://github.com/IlariaSalogni/GeoLing/blob/main/GeoLingIt_Evalita23_Salogni.ipynb)
