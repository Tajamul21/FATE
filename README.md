<div align="center">

<!-- TITLE -->
# **FATE: Focal-modulated Attention Encoder for temperature prediction**

[![arXiv](https://img.shields.io/badge/cs.LG-arXiv:2303.16203-b31b1b.svg)](http://arxiv.org/abs/2408.11336)
[![Website](https://img.shields.io/badge/🌎-Website-blue.svg)](http://diffusion-classifier.github.io)
</div>

This is the official implementation of the arxiv paper [FATE: Focal-modulated Attention Encoder for temperature prediction](https://arxiv.org/abs/2303.16203) by Tajamul Ashraf and Janibul Bashir.
<!-- DESCRIPTION -->
## Abstract

One of the biggest issues facing humanity in the twenty-first century is climate change, as shown by the increasing sea levels, melting glaciers, and frequent storms. Accurate temperature forecasting is crucial for understanding and mitigating its impacts. Cutting-edge data-driven models for temperature forecasting typically employ recurrent neural networks(CNNs), with certain models integrating attention mechanisms. However RNNs sequential processing limits parallelization, especially for longer sequences. In order to do this, we provide a brand-new method for temperature prediction that is based on the FocalNet Transformer architecture. By functioning in a multi-tensor format, the suggested Focal-modulation Attention Encoder (FATE) framework leverages the spatial and temporal nuances of meteorological data characteristics by integrating tensorized modulation. Comparative assessments against existing transformer encoder architectures, 3D CNNs, LSTM, and ConvLSTM demonstrate our model’s superior ability to capture nuanced patterns inherent in the data, particularly in the context of temperature prediction. We also introduce a new labeled dataset, Climate change Parameter dataset (CCPD), which encompasses 40 years of data from J&K region on seven key parameters that influence climate change, supporting further research in this area. Experiments on two real-world benchmark temperature datasets from weather stations in the USA, Canada, and Europe demonstrate accuracy improvements of 12%, 23%, and 28% respectively, compared to existing SOTA models. In addition, we achieved state-of-the-art results on our CCPD dataset with a 24% improvement. To understand FATE, we introduce two modulation scores from the tensorial modulation process. These scores clarify our model’s decision making and key climate change parameters. For reproducible research, we will release the source code, pre-trained FATE model, and CCPD dataset.




## Model architecture
![FATE](images/model_arch.png)


![FATE](images/all_together.jpg)


## Results

![FATE](images/result_europe.png)
The obtained test MAE of the models for USA-Canada dataset averaged over cities (a) and prediction time steps (b).

## Focal Modulation visualization

![FATE](images/result_USA.png)
Modulation visualization for Dallas in USA-Canada dataset.

## Data

In order to download the data, please email to the following address:

t-tashraf@microsoft.com


## Usage
Execute the notebook on colab (Use TPU for FATE): [Experiments_club.ipynb](notebooks/Experiments_club.ipynb)

## Citation
If you use our data and code, please cite the paper using the following bibtex reference:
```
@article{ashraf2024fatefocalmodulatedattentionencoder,
      title={FATE: Focal-modulated Attention Encoder for Temperature Prediction}, 
      author={Tajamul Ashraf and Janibul Bashir},
      year={2024},
      eprint={2408.11336},
      archivePrefix={arXiv},
      primaryClass={cs.LG},
      url={https://arxiv.org/abs/2408.11336}, 
}
```
Thank you for your attention. Cheers!
