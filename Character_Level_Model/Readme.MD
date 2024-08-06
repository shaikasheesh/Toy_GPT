## We have taken a Shakespere data set which is of 1 MB and we train GPT model on this data to generate text which is similar to the input data file

### Here is the config that we have used for building the GPT

* batch_size = 16
* block_size = 256 (which is the context length)
* vocab_size = 65
* n_emb = 128
* num_heads = 6 
* n_layers = 6
* dropout = 0.0
* learning_rate = 1e-3 
* min_lr = learning_rate * 0.1 ( This is calculated because we have used Cosine LR scheduler )

### Additional Implementations which are inspired from Transformers, GPT2 & LLama Research Papers

* Weights are initialized with std == 0.02 and mean == 0
* AdamW optimizer with weight decay of 0.1 and betas (0.9,0.95) is used
* Normalized the Gradients in the Training loop 


#### Note: This Implementation work is done with help of Andrej Karpathy nanoGPT repo 
