# Finetuning-Whisper

This repository is for fine-tuning Whipser which is one of ASR models released by OpenAI.

Paper link: [https://arxiv.org/abs/2212.04356](https://arxiv.org/abs/2212.04356)

# Environments

Colab Pro V100 GPU

## Input

pair of audio sample and transcribed text(json format)

## Output

transcribed text

## Model

Whipser-small (# of parameters: 244M, sampling rate: 16khz)

## Dataset Configuration

We used Mozilla foundation's common voice 11 hindi dataset.

About 6500 training dataset, About 2900 Test dataset

## Setting Experiments

epoch:10, batch size: 16, lr: 1e-5

After fine-tuning Whisper model, we calculated WER for each 1,000 step.

## Result

WER 33

## Limitation

Because of storage and GPU shortage, I had no choice but to utilize Hindi dataset rather than Korean or English.

# References

[UNIT 1. Working with audio data](https://huggingface.co/learn/audio-course/chapter1/introduction)

[UNIT 2. A Gentle Introduction to Audio Applications](https://huggingface.co/learn/audio-course/chapter2/introduction)

[UNIT 3. Transformer Architectures for Audio](https://huggingface.co/learn/audio-course/chapter3/introduction)

[UNIT 5. Automatic Speech Recognition](https://huggingface.co/learn/audio-course/chapter5/introduction)
