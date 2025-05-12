# Small LLMs Can Rock! Difficulty-Aware CoT Distillation for SQL Generation

This repository is the official implementation of [Small LLMs Can Rock! Difficulty-Aware CoT Distillation for SQL Generation]. 

## Requirements

python==3.8.5

torch==2.4.0

openai==0.28

tqdm==4.66.5

transformers==4.46.3

sqlparse==0.5.3

datasets==2.14.6

trl==0.10.1

accelerate==1.0.1



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
Note that during inference, you need to first generate CoTs. Next, you need to remove the code related to CoT generation. Finally, you need to use the code related to SQL generation.

## Evaluation

To evaluate the proposed framework, please run this command:

```test
sh src/test.sh
```

## Pre-trained Models

You can download pretrained models here:

https://huggingface.co/Qwen/Qwen2.5-Coder-3B-Instruct

https://huggingface.co/meta-llama/Llama-3.2-3B-Instruct
