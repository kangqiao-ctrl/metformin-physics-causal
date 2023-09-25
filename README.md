# Causal Prior-Embedded Physics-Informed Neural Networks
Data and code associated with the manuscript "Causal Prior-Embedded Physics-Informed Neural Networks and a Case Study on Metformin Transport in Porous Media."

This repository contains:
1. The augmented datasets generated by Phydrus/Hydrus-1D
   - **df_causal.parquet**:  Used for causal effect estimation;
   - **df_NN.parquet**: Used for neural network experiments.
2. A neural network framework /w causal weight initialization and causal regularization (Ref1)
   - **model_causal_reg.py**: Main program, PyTorch required
   - **set_random_seed.py**: Randomizer file.
3. [NNI](https://github.com/microsoft/nni) (Ref2) configuration related files. 
   - **search_space.json**: Example search space configuration for NNI
   - **config-example.yaml**: Example experiment configuration for NNI
   For a detailed instruction on NNI, please refer to [NNI Documentation](https://nni.readthedocs.io/en/stable/)

Due to the size and format of the files mentioned below, we are considering uploading the following files associated with this paper to **Zenodo**:

1. Original Hydrus-1D files (from the column experiment data)
2. Phydrus files (For generating augmented data)
3. Our NNI experiment results (1,440 runs)

We will provide an update here before Sep 28, 2023.

References

(1) Kancheti, S. S., Reddy, A. G., Balasubramanian, V. N., & Sharma, A. (2021). Matching learned causal effects of neural networks with domain priors. arXiv preprint arXiv:2111.12490.

(2) Microsoft. (2021). Neural Network Intelligence (Version 2.0) [Computer software]. 
