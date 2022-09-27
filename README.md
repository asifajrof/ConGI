



# Deciphering Spatial Domains by Integrating Histopathological Image and Transcriptomics via Contrastive Learning 




## Overview
We propose a novel method ConGI to accurately decipher spatial domains by integrating gene expression and histopathologi-cal images, where the gene expression is adapted to image infor-mation through contrastive learning. We introduce three contrastive loss functions within and between modalities to learn the common semantic representations across all modalities while avoiding their meaningless modality-private noise information. The learned rep-resentations are then used for deciphering spatial domains through a clustering method. By comprehensive tests on tumor and normal spatial transcriptomics datasets, ConGI was shown to outperform existing methods in terms of spatial domain identification. More importantly, the learned representations from our model have also been used efficiently for various downstream tasks, including trajectory inference, clustering, and visualization. 

![(Variational) gcn](framework.bmp)


## Requirements
Please ensure that all the libraries below are successfully installed:

- **torch 1.7.1**
- CUDA Version 10.2.89
- scanpy 1.8.1
- mclust








## Run ConGI the example data.

```

python main.py --dataset her2+  --name E1

```


## output

The clustering cell labels will be stored in the dir [output](https://github.com/biomed-AI/ConGI) /dataname_pred.csv. 



## Datasets

The spatial transcriptomics datasets that support the findings of this study are available here:
(1) human HER2-positive breast tumor ST data https://github.com/almaan/HER2st/. 
(2) The LIBD human dorsolateral prefrontal cortex (DLPFC) data was acquired with 10X Visium composed of spatial transcriptomics data acquired from twelve tissue slices (http://research.libd.org/spatialLIBD/).
(3) The mouse brain anterior section from 10X Visium (https://www.10xgenomics.com/resources/datasets). 
(4) the human epidermal growth factor receptor (HER) 2-amplified (HER+) invasive ductal carcinoma (IDC) (https://support.10xgenomics.com/spatial-gene-expression/datasets). 




## Citation

Please cite our paper:

```

@article{zengys,
  title={Deciphering Spatial Domains by Integrating Histopathological Image and Tran-scriptomics via Contrastive Learning },
  author={Yuansong Zeng1,#, Rui Yin3,#, Mai Luo1, Jianing Chen1, Zixiang Pan1, Yutong Lu1, Weijiang Yu1* , Yuedong Yang1,2*},
  journal={biorxiv},
  year={2022}
 publisher={Cold Spring Harbor Laboratory}
}

```
