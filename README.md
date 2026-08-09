# Continuous Sign Language Recognition and Translation

A hybrid deep learning framework for continuous sign language recognition and translation using fused I3D and MediaPipe features, Multi-Scale CNN, BiLSTM, and Transformer Decoder.

## Overview

This project presents a deep learning-based system for recognizing continuous sign language sequences and generating sentence-level German text.

The system uses pre-extracted I3D motion features and MediaPipe pose features from the RWTH-PHOENIX-Weather 2014T dataset. These features are fused and processed using a Multi-Scale CNN and BiLSTM encoder, followed by a Transformer Decoder for sentence generation.

The generated German text is further translated into English using the MarianMT neural machine translation model.

## Key Features

- I3D motion feature extraction
- MediaPipe pose feature extraction
- Multimodal feature fusion
- Multi-Scale CNN with kernel sizes 3, 5 and 7
- 2-layer Bidirectional LSTM
- 4-layer Transformer Decoder
- Beam Search decoding
- German-to-English translation using MarianMT
- WER and BLEU evaluation
- Interactive Gradio web application

## Model Pipeline

Sign Language Video

→ I3D Features + MediaPipe Features

→ Feature Fusion

→ Linear Projection

→ Multi-Scale CNN

→ BiLSTM Encoder

→ Transformer Decoder

→ Beam Search

→ German Text

→ MarianMT

→ English Translation

## Dataset

The system is trained and evaluated using the RWTH-PHOENIX-Weather 2014T dataset.

The dataset contains continuous German Sign Language videos from weather forecast broadcasts along with corresponding German sentence translations.

### Dataset Split

| Split | Samples |
|------|--------:|
| Training | 7096 |
| Validation | 519 |
| Test | 642 |

## Results

| Metric | Result |
|--------|-------:|
| WER | 0.7504 |
| BLEU-1 | 0.3747 |
| BLEU-2 | 0.2708 |
| BLEU-3 | 0.2102 |
| BLEU-4 | 0.1652 |

## Technologies

- Python
- PyTorch
- I3D
- MediaPipe
- CNN
- BiLSTM
- Transformer
- MarianMT
- Gradio

## Authors

- Author 1
- Author 2
- Author 3
