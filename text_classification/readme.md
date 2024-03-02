# Fine-Tuned Emotion Classification Model

## Model Description

This model is a fine-tuned version of DistilBERT-base-uncased on the emotion dataset. It has been trained to classify text inputs into different emotion categories.

## Intended Uses & Limitations

**Intended Uses:**
- Text classification tasks where emotions need to be identified.
- Sentiment analysis applications.
- Emotion detection in customer feedback or social media posts.

**Limitations:**
- Performance may vary on data significantly different from the training dataset.
- Limited to the emotion categories present in the training data.
- May not capture nuanced or complex emotions effectively.

## Training and Evaluation Data

*More information needed.*

## Training Procedure

### Training Hyperparameters

The following hyperparameters were used during training:
- Learning Rate: 2e-05
- Train Batch Size: 64
- Eval Batch Size: 64
- Seed: 42
- Optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- Learning Rate Scheduler Type: Linear
- Number of Epochs: 10

### Training Results

| Training Loss | Epoch | Step | Validation Loss | Accuracy | F1    |
|---------------|-------|------|-----------------|----------|-------|
| 0.7744        | 1.0   | 250  | 0.2544          | 0.9185   | 0.9189|
| 0.1925        | 2.0   | 500  | 0.1659          | 0.9355   | 0.9354|
| 0.1285        | 3.0   | 750  | 0.1505          | 0.936    | 0.9367|
| 0.1008        | 4.0   | 1000 | 0.1402          | 0.942    | 0.9419|
| 0.0822        | 5.0   | 1250 | 0.1429          | 0.9405   | 0.9405|
| 0.0676        | 6.0   | 1500 | 0.1512          | 0.9395   | 0.9396|
| 0.0562        | 7.0   | 1750 | 0.1641          | 0.9385   | 0.9384|
| 0.046         | 8.0   | 2000 | 0.1698          | 0.935    | 0.9351|
| 0.0379        | 9.0   | 2250 | 0.1705          | 0.939    | 0.9389|
| 0.0334        | 10.0  | 2500 | 0.1714          | 0.9395   | 0.9395|

## Framework Versions

- Transformers: 4.38.1
- PyTorch: 2.1.0+cu121
- Datasets: 2.18.0
- Tokenizers: 0.15.2

For more details and to use the model, visit [here](https://huggingface.co/JayShah07/Tweet-finetuned-emotion-classification).

