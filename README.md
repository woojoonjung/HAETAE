# HAETAE

This code is the official implementation of our SIGIR'25 paper: HAETAE: In-domain Table Pretraining with Header Anchoring.

requirements for training and experiment is as followed
> torch \
  transformers \
  tensorboard \
  pandas \
  scikit-learn \
  numpy==1.26.4
   
### Training
The datasets we used in training can be downloaded from https://webdatacommons.org/structureddata/schemaorgtables/2023/ 


We utilized top100 subset of Product and Movie to create pretraining data.

To train the model, run the train.py script.
For example :
> python train.py \
  --data_path ./data/pretraining_data_movie.jsonl  \
  --output_dir ./models/movie_haetae

### Experiment
We uploaded a sample test data consisted of multi-lingual json objects and a jupyter notebook file for masked prediction experiment.

### Citation

If you find this repository useful, please consider citing our paper:

```bibtex
@inproceedings{jung2025haetae,
  title={HAETAE: In-domain Table Pretraining with Header Anchoring},
  author={Jung, Woojun and Yoon, Susik},
  booktitle={Proceedings of the 48th International ACM SIGIR Conference on Research and Development in Information Retrieval},
  pages={3065--3069},
  year={2025}
}
