# -Efficient-Fine-Tuning-of-Large-Language-Models-for-Dialogue-Summarization

This project is from Coursera's couse "Generative AI with Large Language Model" 

-In this project, I utilized PyTorch and the HuggingFace transformers library to build a fine-tuning pipeline for Large Language Models (LLMs). The target model used for this process was Google's FLAN-T5. The fine-tuning process was explored through two distinct methods: full fine-tuning and Parameter Efficient Fine-Tuning (PEFT).

-PEFT, which includes techniques like Low-Rank Adaptation (LoRA), was employed to reduce the computational burden of fine-tuning, enabling model adaptation on lesser resources, sometimes as low as a single GPU. The output of this process was a significantly smaller "LoRA adapter" that could be combined with the original LLM for inference tasks, providing a memory-efficient solution.

-The model's performance was assessed both qualitatively (via human evaluation) and quantitatively (using the ROUGE metric for summarization tasks), and compared across the original LLM, a fully fine-tuned version, and the PEFT model. While the PEFT model achieved slightly lower performance metrics, the computational efficiency gain substantiated its usage. Finally, I leveraged AWS S3 for efficient model checkpoint storage and retrieval, further enhancing the operational efficiency of the PEFT model.
