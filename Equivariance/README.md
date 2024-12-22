# Tutorials

```

├──  al         - contains code related to Active Sampling methods
│
├──  dataset    - contains data for training
|                  (data needs to be saved in .pt format)
│ 
├──  datasets   - contains code for preparing dataset
│ 
├──  models     - code of baseline models and our BGNN
│   
├──  utils       - contains general utility functions
|
├──  runs       - for saving the results, 
|                the name of folder should be same as selection_method in run.sh file
|
│    └── random  - for random method
│       └── run1
|            └── init_set.npy   - file containing initial labeled indices(user should prepare)
|
│    └── unc_div - for our method
|        └── run1
             └──    tensor.pt  - similarity matrix (compute using compute_sim_mat.py)
|            └── init_set.npy   - file containing initial labeled indices  
|
├── run.sh        - for configuring training hyper parameters
|
|
├── compute_sim_mat.py        - for computing similarity matrix(our and soap method)
|                               * save the obtained tensor.pt file in appropriate folder inside runs/ *
|                               * use the function: compute_uncertainty_diversity_gpu for faster computation*
|
|
├── train.py
```
