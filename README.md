# STEGASURAS
STEGanography via Arithmetic coding and Strong neURAl modelS

This repository contains implementations of the steganography algorithms from ["Neural Linguistic Steganography," Zachary M. Ziegler*, Yuntian Deng*, Alexander M. Rush](https://arxiv.org/abs/1909.01496).

There is a breaking change in pytorch 1.2, make sure to use pytorch 1.0 as in requirements.txt.

## Language model

Experiments in the paper use the medium (345M parameter) GPT model via [pytorch_transformers](https://github.com/huggingface/pytorch-transformers). For compute reasons the default in this code base is the small version but the medium or large versions can be used by changing the `model_name` parameter of `get_model`.

## Algorithms

The steganography algorithms implemented are:
1. Our proposed arithmetic coding-based algorithm]

An example of encoding and decoding a message is in `run_single.py`. The algorithm used is determined by the `mode` parameter.
