## Uplift Modelling for Dataset with 20 Confounders
### Results:
- 'train_result_x20.csv' is the training result and the comparison with baseline performance
- 'valid_result_x20.csv' is the validation result and the comparison with baseline performance
### Notes:
0. Running '0_ate_weighting.ipynb' to obtain causal weighting for each feature, the output is 'feats_ate_x20.xlsx'.
1. Running '1_feature_correlations_BNEstimator.ipynb' to obtain nodes and edges from Bayesian Net, the output is 'edge_index_data_20.csv'.
2. Running '2_node_embeddings.ipynb' to obtain node embeddings by DeepWalk and Node2Vec, the output is 'deepwalk_10d_x20.model' and 'Node2Vec_10d_x20.model'.
3. Running 'causal_embedding(10d)_ ate(21d)_ x20_.ipynb' and 'causal_embedding(10d)_ unweighted_ x20_.ipynb' in this repository to perform **Causal-weighted and Unweighted uplift modelling, respectively**.


