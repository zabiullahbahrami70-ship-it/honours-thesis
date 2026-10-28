# Multimodal Harmful Content Detection: Comparing Optimisation Strategies and Their Impact on Explainability

Honours thesis code (RMIT University). Compares four optimisation strategies for a CLIP ViT-B/32 classifier on hateful meme detection, evaluating classification (AUROC) and explanation faithfulness (ERASER comprehensiveness and sufficiency against a matched random baseline).

Strategies: full fine-tuning, LoRA, QLoRA, and supervised contrastive learning with LoRA.

## Repository contents

- `notebooks/Project_2_Thesis_Notebook.ipynb`: the full experiment notebook (training, evaluation, explanations, statistics).
- `requirements.txt`: Python dependencies.

## Data

The dataset is the Hateful Memes Challenge (Kiela et al., 2020). It is **not included** in this repository. Obtain it from the official source and follow its licence terms. Place the files in the paths the notebook expects (see the Paths cell).

The notebook's saved outputs have been cleared for images that show dataset content. Charts and tables are retained.

## Running

The notebook was developed in Google Colab (T4 and L4 GPUs). To reproduce:

1. Open the notebook in Colab and set the runtime to GPU.
2. Store your Weights & Biases key in Colab Secrets as `wandb_key`, or remove the W&B cells.
3. Run the cells in order. Training writes checkpoints to Google Drive.

Random seed: 42. Each strategy was trained once, so results reflect a single run per strategy.

## Licence

To be added.

## Citation

To be added after submission.
