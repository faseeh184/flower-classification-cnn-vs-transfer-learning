# Flower Image Classification: CNN vs Transfer Learning

Compares a CNN trained from scratch with pretrained models (VGG19, ResNet50) for classifying flower images (daisy, dandelion, roses, sunflowers, tulips).

## Results (validation accuracy)
| Model | Accuracy |
|---|---|
| Custom CNN (from scratch) | 24.5% (did not learn) |
| VGG19 (transfer learning) | 53% |
| **ResNet50 (transfer learning)** | **62.6%** |

## What I learned
- The from-scratch CNN stayed near chance level on this small dataset.
- Pretrained features helped a lot: ResNet50 more than doubled the scratch model.
- Next steps: data augmentation, fine-tuning the last layers, more epochs, and learning-rate scheduling.

## Tech stack
Python · TensorFlow / Keras · NumPy · Matplotlib

## Run it
```bash
pip install -r requirements.txt
jupyter notebook flower_classification-1008.ipynb
```

## Author
Faseeh · [LinkedIn](https://www.linkedin.com/in/faseeh-uddin-mohammed-a0455823b)
