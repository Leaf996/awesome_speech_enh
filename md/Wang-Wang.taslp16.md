# A Joint Training Framework for Robust Automatic Speech Recognition
## Abstract
- Robustness against noise and reverberation is critical for ASR systems deployed in real-world environments. In addition, we apply `sequence training` to the jointly trained DNN so that the linguistic information contained in the acoustic and language models can be back-propagated to influence the separation frontend at the training stage.
## Introduction
- Speech separation and recognition are not two independent tasks and they can clearly benefit from each other.
## System Description
- Speech Separation
    - It is suggested that the IRM is likely to be better training target for supervised speech separation. Therefore, we utilize DNNs to estimate the IRM in this study.
- Acoustic Modeling
    - However, mel-spectrogram itself is not robust to noise and reverberation.
- Joint Training
    - In our approach, parameter initialization is critical before joint training.
- Sequence-Discriminative Training
    -  As automatic speech recognition is itself a sequence classification problem, it is sensible to optimize the sequence-discriminative criterion to better capture the essence of this problem.
- Unsupervised Adaptation
    - Adaptation is commonly performed on well-trained acoustic models to compensate the differences between training and test conditions.