# My Paper Title

This repository is the official implementation of [Small LLMs Can Rock! Difficulty-Aware CoT Distillation for SQL Generation]. 

## Difficulty-Aware CoT Generation

For generating difficulty levels in the training set, please run this command:

```label
python src/label.py
```
For generating difficulty-aware CoTs, please run this command:

```cot
python src/cot.py
```

## Stepwise CoT Distillation

For model training, please run this command:

```train
sh src/train.sh
```

For model inference, please run this command:

```inference
sh src/eval.sh
```

## Evaluation

To evaluate the proposed framework, please run this command:

```test
python test.py
```

## Pre-trained Models

You can download pretrained models here:

https://huggingface.co/Qwen/Qwen2.5-Coder-3B-Instruct
https://huggingface.co/meta-llama/Llama-3.2-3B-Instruct



## Contributing

>📋  The license is CC BY 4.0.
