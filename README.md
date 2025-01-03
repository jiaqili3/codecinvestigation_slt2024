# Investigating neural audio codecs for speech language model-based speech generation
This is a repository for our SLT2024 paper: Investigating neural audio codecs for speech language model-based speech generation.
Paper link: [link](https://arxiv.org/abs/2409.04016)
## Abstract
Neural audio codec tokens serve as the fundamental building blocks for speech language model (SLM)-based speech generation. However, there is no systematic understanding on how the codec system affects the speech generation performance of the SLM. In this work, we examine codec tokens within SLM framework for speech generation to provide insights for effective codec design. We retrain existing high-performing neural codec models on the same data set and loss functions to compare their performance in a uniform setting. We integrate codec tokens into two SLM systems: masked-based parallel speech generation system and an auto-regressive (AR) plus non-auto-regressive (NAR) model-based system. Our findings indicate that better speech reconstruction in codec systems does not guarantee improved speech generation in SLM. A high-quality codec decoder is crucial for natural speech production in SLM, while speech intelligibility depends more on quantization mechanism. 
## Key Results
We explored various neural codec systems for the SLM-driven speech generation task. Our investigation included training our own baseline codec systems, as well as variants based on existing high-performing codec systems, including Encodec, Vocos, and DAC. We integrated the codec tokens from these codec systems into two types of SLM-based speech generation systems: masked-based parallel speech generation and AR + NAR models-based text to speech generation systems. Our experiment results revealed that DAC models perform exceptionally well overall for SLM-based speech generation. Vocos served as a competitive vocoder, demonstrating similar performance as the DAC decoder. Interestingly, we observed that the speech reconstruction quality was highly correlated with the naturalness of the generated speech, but this correlation did not hold true for speaker similarity and speech intelligibility.

## Citations
```
@inproceedings{codecinvestigation,
title={Investigating Neural Audio Codecs for Speech Language Model-Based Speech Generation}, 
author={Jiaqi Li and Dongmei Wang and Xiaofei Wang and Yao Qian and Long Zhou and Shujie Liu and Midia Yousefi and Canrun Li and Chung-Hsien Tsai and Zhen Xiao and Yanqing Liu and Junkun Chen and Sheng Zhao and Jinyu Li and Zhizheng Wu and Michael Zeng},
year={2024},
booktitle    = {{SLT}},
}
```