# Generate TV Scripts
In this project, I generate your own Seinfeld TV scripts using RNNs. I use a Seinfeld dataset of scripts from 9 seasons. The Neural Network I build will generate a new, "fake" TV script.


## Project Information

### Contents

- Get the Data
- Explore the Data
- Implement Pre-processing Functions
	- Lookup Table
	- Tokenize Punctuation
- Pre-process all the data and save it
- Check Access to GPU
- Input
	- Batching
	- Test your dataloader
	- Sizes
	- Values
- Build the Neural Network
	- Define forward and backpropagation
- Neural Network Training
	- Train Loop
	- Hyperparameters
	- Train 
- Generate TV Script
	- Generate text
	- Generate a new script
  
  ### Model
| Layer | Input Dimension | Output Dimension |
| ----- | --------------- | ---------- |
|Embedding|Vocab Size| 300 |
|LSTM|300|256|
|FC|256|Vocab Size|

### Hyperparameters
|Data Parameter|Value|
|--------------|------|
|sequence_length| 10|
|batch_size| 128 |

|Training Parameter|Value|
|------------------|-----|
|num_epochs|10|
|learning_rate|0.001|
|embedding_dim|300|
|hidden_dim|256|
|n_layers(Number of RNN Layers)|3|
