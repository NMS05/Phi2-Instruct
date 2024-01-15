# Phi2-Instruct

## Model Description
The Phi2-Instruct model is trained on the [mosaicml/dolly_hhrlhf](https://huggingface.co/datasets/mosaicml/dolly_hhrlhf) dataset in a supervised fashion using the Huggingface SFT Trainer. The base model is the [Phi-2](https://huggingface.co/microsoft/phi-2) Small Language Model (SLM) released by Microsoft under the [MIT license](https://huggingface.co/microsoft/phi-2/resolve/main/LICENSE).

## Training Details
* Base model: Phi-2
* Base model precision: INT8
* PEFT method: LoRA (rank=16)
* Context Length = 2048

## Weights
The LoRA weights for the Phi2-Instruct model can be found in [releases](https://github.com/NMS05/Phi2-Instruct/releases). Download, Unzip and modify the path in Phi2_Instruct.ipynb for inference.

## Scripts
* Phi2_Finetune.ipynb - Jupyter notebook to train Phi-2 model on dolly_hhrlhf using SFT.
* Phi2_Instruct.ipynb - Jupyter notebook for inference with Phi2-Instruct.

## Sample Output
<img src=https://github.com/NMS05/Phi2-Instruct/blob/main/inference.png width="950" height="300">

## Reference
[DataCamp - How to train a LLM?](https://www.datacamp.com/tutorial/how-to-train-a-llm-with-pytorch)
