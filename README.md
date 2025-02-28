# HAETAE

requirements for training and experiment is as followed
> torch \
  transformers \
  tensorboard \
  pandas \
  scikit-learn \
  fasttext \
  numpy==1.26.4
   
#### Training
The datasets we used in training can be downloaded from https://webdatacommons.org/structureddata/schemaorgtables/2023/ 
We utilized top100 subset of Product and Movie to create pretraining data.

To train the model, run the train.py script.
For example :
> python train.py \
  --data_path ./data/pretraining_data_movie.jsonl  \
  --output_dir ./models/movie_complete

### Experiment
We uploaded a sample test data consisted of multi-lingual json objects and a jupyter notebook file for masked prediction experiment.