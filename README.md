# ML-Models (Part #3)
This repository contains the third and last part of the solution for the challenge "KDD BR Competition 2022" of the team Artificial Psycho Killer.

## Image sequences
During the challenge it was noticed how images from the datasets were inserted from a video, as a consequence, there was a sequence in the images. To find the sequence, just run the code `/src/find_sequence.ipynb` and then `/src/create_sequence_ids.ipynb`.

Next to that, we create the folds, segregating them by sequence, the file for generating the folds is `/src/kfold_gen.ipynb`.

## Models

Our final solution was a stacking of 15 different models, that use the features generated in the part #1 and #2 of our solution, these models can be found at `/src/L0_models`, the final stacking can be found at `/src/L1_models`.

To gerenate our final solution, just clone this repo and run the file `/src/L1_models/stacking.ipynb`.

### Level-0 Models

#### XGBoost
- xgb_seq_001
- xgb_seq_002
- xgb_seq_003
- xgb_seq_004
- xgb_seq_005
- xgb_seq_006
- xgb_seq_008
- xgb_seq_009
- xgb_seq_011
- xgb_onlylag

#### LightGBM
- lgb_seq_003

#### Catboost
- cat_seq_001
- cat_seq_003
- cat_onlylag