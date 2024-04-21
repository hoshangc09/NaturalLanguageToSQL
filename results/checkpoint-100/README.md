# Checkpoint-100 Contents

This folder contains various configuration and model files for the Checkpoint-100 stage of the SQL Query Generation project. These files represent the state of the model at the 100th step of training.

## Files Description

- `added_tokens.json`: Stores additional tokens that the model might use during tokenization or sequence generation.
- `config.json`: Contains the model's configuration settings including hyperparameters.
- `generation_config.json`: Specifies settings related to the generation aspect of the model.
- `model.safetensors`: The binary file storing the weights and biases of the model at this checkpoint.
- `special_tokens_map.json`: Maps special tokens to the roles they serve in the tokenization process.
- `spiece.model`: A SentencePiece model file that assists in tokenizing inputs to the model.
- `tokenizer_config.json`: Configuration for the tokenizer, detailing how text strings are converted into tokens.

These files are essential for resuming training from this checkpoint, conducting further experiments, or for deployment in a production environment.

