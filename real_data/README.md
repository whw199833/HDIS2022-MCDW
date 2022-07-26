This is the `Data`, `Notebooks` and `Results` for the experiment with the `real_world_dataset`

## Data
`real_world_dataset`: [criteo-uplift-v2.1.csv](https://1drv.ms/u/s!AuZMIQsKXGynq4lSIGaY3wZGUHBXXQ?e=lM9pAm)

## Notebooks
- Running '0_ate_weighting.ipynb' to obtain causal relationships between the target and each feature, the output is 'feats_ate_x13.xlsx'.
- Running '1_feature_correlations_BNEstimator.ipynb' to obtain feature correlations from Bayesian Net, the output is 'edge_index_criteo.csv'.
- Running '2_node_embeddings.ipynb' to obtain node embeddings by DeepWalk and Node2Vec, the output is 'deepwalk_10d_x13.model' and 'Node2Vec_10d_x13.model'. 
- Running '3_causal_weighting_embedding(10d)_ate(13d).ipynb' to perform **Causal-weighted, Equal-weighted and Unweighted Uplift Modelling**.
