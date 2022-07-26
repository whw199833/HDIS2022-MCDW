## Uplift Modelling for Dataset with 9 Confounders
### Results:
- 'train_result_x9.csv' is the training result and the comparison with baseline performance
- 'valid_result_x9.csv' is the validation result and the comparison with baseline performance
### Notes:
Please navigate to the [real_data repository](https://github.com/whw199833/Uplift-Modeling-based-on-Graph-Neural-Network-Combined-with-Causal-Weighting/tree/main/real_data) to obtain the necessary notebooks: '0_ate_weighting.ipynb', '1_feature_correlations_BNEstimator.ipynb' and '2_node_embeddings.ipynb'

0. Running '0_ate_weighting.ipynb' to obtain causal weighting for each feature, the output is 'feats_ate_x9.xlsx'.
1. Running '1_feature_correlations_BNEstimator.ipynb' to obtain nodes and edges from Bayesian Net, the output is 'edge_index_data_9.csv'.
2. Running '2_node_embeddings.ipynb' to obtain node embeddings by DeepWalk and Node2Vec, the output is 'deepwalk_10d_x9.model' and 'Node2Vec_10d_x9.model'. 
3. Running 'causal_embedding(10d)_ ate(10d)_ x9_.ipynb' and 'causal_embedding(10d)_ unweighted_ x9_.ipynb' in this repository to perform **Causal-weighted and Unweighted uplift modelling, respectively**.

