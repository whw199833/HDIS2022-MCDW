## Uplift Modelling for dataset with 5 confounders
### Results:
- 'train_result_x5.csv' training results and comparison with baseline performance
- 'valid_result_x5.csv' validation results and comparison with baseline performance
### Notes:
0. Running '0_ate_weighting.ipynb' to obtain causal weighting for each feature, the output is 'Synthetic_feats_ate.xlsx'
1. Running '1_feature_correlations_BNEstimator.ipynb' to obtain nodes and edges from Bayesian Net, the output is 'synthetic_edge_index.csv'
2. Running '2_node_embeddings.ipynb' to obtain node embeddings by DeepWalk and Node2Vec, the output is 'synthetic_deepwalk_10d.model' and 'synthetic_Node2Vec_10d.model' 
3. Running 'causal_embedding(10d)_ ate(6d)_ .ipynb' and 'causal_embedding(10d)_ unweighted_.ipynb' in this repository to perform **Causal-weighted and Unweighted uplift modelling**, respectively 