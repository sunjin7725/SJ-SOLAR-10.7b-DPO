# SJ-Donald/SJ-SOLAR-10.7b-DPO

SJ-Donald/SJ-SOLAR-10.7b-DPO is fine-tuned using DPO method.

## HuggingFace

* [SJ-Donald/SJ-SOLAR-10.7b-DPO](https://huggingface.co/SJ-Donald/SJ-SOLAR-10.7b-DPO)

## Environment

Using **Google CoLab A100**

## Base model

* [SJ-Donald/SOLAR-10.7B-slerp](https://huggingface.co/SJ-Donald/SOLAR-10.7B-slerp)

## Datasets

* [SJ-Donald/orca-dpo-pairs-ko](https://huggingface.co/datasets/SJ-Donald/orca-dpo-pairs-ko)

## How to use

```Python
import torch
from transformers import AutoModelForCausalLM, AutoTokenizer

repo = 'SJ-Donald/SJ-SOLAR-10.7b-DPO'

tokenizer = AutoTokenizer.from_pretrained(repo)
model = AutoModelForCausalLM.from_pretrained(
    repo,
    return_dict=True,
    torch_dtype=torch.float16,
    device_map='auto'
)
```

---
license: cc-by-nc-4.0
tags:
- DPO
---
