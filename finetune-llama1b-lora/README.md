# Main Idea
- How Korean benchmark of 1B model will change?

## Dataset

- Dataset from AIHub to train LLM
- Both corpus and SFT datasets exist

## Methodology

- Use LoRA technique (training small, efficient adapter layers)
- Large Korean pre-training corpus as the dataset in LoRA

## Evaluation

- Use KoBEST for the following metircs:
  - kobest_boolq: Y/N Question-Answering
  - kobest_copa: Causal Reasoning
  - kobest_hellaswag: Commonsense
  - kobest_sentineg: Sentiment

## Result

- No improvements at all

## Refelections

- Model size is too small to have emergent abilities of LLM reported in recent papers
  - Increase the model size to 3B or more
- Training loss haven't decreased a lot as step increases
  - Adjust hyperparameters


## Note

- Training took almost 10 hours with A100 GPU in Colab
