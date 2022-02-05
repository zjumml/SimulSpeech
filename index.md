---
layout: default
---

# SimulSpeech: End-to-End Simultaneous Speech to Text Translation


## Abstract

In this work, we develop SimulSpeech, an end-to-end simultaneous speech to text translation system which translates speech in source language to text in target language concurrently. SimulSpeech consists of a speech encoder, a speech segmenter and a text decoder, where 1) the segmenter builds upon the encoder and leverages a connectionist temporal classification (CTC) loss to split the input streaming speech in real time, 2) the encoder-decoder attention adopts a wait- strategy for simultaneous translation. SimulSpeech is more challenging than previous cascaded systems (with simultaneous automatic speech recognition (ASR) and simultaneous neural machine translation (NMT)). We introduce two novel knowledge distillation methods to ensure the performance: 1) Attention-level knowledge distillation transfers the knowledge from the multiplication of the attention matrices of simultaneous NMT and ASR models to help the training of the attention mechanism in SimulSpeech; 2) Data-level knowledge distillation transfers the knowledge from the full-sentence NMT model and also reduces the complexity of data distribution to help on the optimization of SimulSpeech. Experiments on MuST-C English-Spanish and English-German spoken language translation datasets show that SimulSpeech achieves reasonable BLEU scores and lower delay compared to full-sentence end-to-end speech to text translation (without simultaneous translation), and better performance than the two-stage cascaded simultaneous translation model in terms of BLEU scores and translation delay.

We did not release the source codes since our model has been transferred to some products of the company.

  
## Authors
- Yi Ren (Zhejiang University) rayeren@zju.edu.cn
- Jinglin Liu (Zhejiang University) jinglinliu@zju.edu.cn
- Xu Tan (Microsoft Research) xuta@microsoft.com
- Chen Zhang (Zhejiang University) zc99@zju.edu.cn
- Tao Qin (Microsoft Research) taoqin@microsoft.com
- Zhou Zhao (Zhejiang University) zhaozhou@zju.edu.cn
- Tie-Yan Liu (Microsoft Research) tyliu@microsoft.com
