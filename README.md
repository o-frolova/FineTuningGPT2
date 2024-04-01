# FineTuningGPT2
## TASK
Using a pre-trained GPT2 model, perform fine-tuning on WikiText dataset, measure quality with BLEU metric, collect and build charts describing dynamics of training. 
Fine-tuning must be performed two variances:
* Full fine-tuning pipeline of GPT2 model on WikiText
* LoRA fine-tuning pipeline of GPT2 model on WikiText
## RESULTS
<b>Note:</b>

* <b>Training area:</b>

| Model                | loss            |
|----------------------|-----------------|
| Full tuning          | 3.0796          |
| LoRA                 | 3.5249          |

  Model with full tunning has a lower learning loss, which may indicate better model performance during training. However, learning loss is not always the only indicator of model quality, and other metrics must also be taken into account.
  </p>

* <b>BLEU Score:</b>

| Model                | BLEU Score   |
|----------------------|--------------|
| Full tuning          | 0            |
| LoRA                 | 0.001259     |

  Model with LoRA shows a small but non-zero BLEU score value, while Model with full tunning has a BLEU score value of 0. This may indicate that Model with LoRA gives slightly better results in evaluating the quality of the generated text.

* <b>Learning rate:</b>

| Model                | Sample processing speed per second   |
|----------------------|--------------------------------------|
| Full tuning          | 15.429                               |
| LoRA                 | 14.052                               |

  Model with full tunning also shows a slightly higher sample processing rate per second, which can be an important factor, especially when training on large amounts of data.


Overall, although Model with full tunning has lower learning loss and higher sample processing speed, Model with LoRA has shown a slight improvement in BLEU estimation, which may indicate some advantages in the quality of text generation.
