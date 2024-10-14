# An LLM-based Framework for Fingerprinting Internet-connected Devices

This repository includes code used for training and evaluating transformer-based
language models on banners obtained from global Internet scans, as presented in
the paper [An LLM-based Framework for Fingerprinting Internet-connected Devices](https://doi.org/10.1145/3618257.3624845).

The code is intended for academic research and educational purposes only. To
request access, please contact Armin Sarabi at [arsarabi@umich.edu](mailto:arsarabi@umich.edu)
from your institutional email address. Please include a brief description of
your project and how your intend to use the code with your request.

Note that trained models are publicly available on the HuggingFace Hub, and can
be used to generate device embeddings for downstream learning tasks, or further
fine-tuned on downstream applications. Currently, the following models are
available:

- [roberta-base-banner](https://huggingface.co/arsarabi/roberta-base-banner): A
  RoBERTa masked language model trained on banners from all protocols available
  in the [Censys Universal Internet BigQuery Dataset](https://support.censys.io/hc/en-us/articles/360056063151-Universal-Internet-BigQuery-Dataset).
- [roberta-embedding-http](https://huggingface.co/arsarabi/roberta-embedding-http):
  A model fine-tuned on HTTP banners (headers) using a contrastive loss function
  to generate temporally stable embeddings.

