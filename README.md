# Project Acronym

**Concordia University, Decathlon**

Hasib Zunair

[[`Paper`](link)] [[`Project`](link)] [[`Demo`](#4-demo)] [[`BibTeX`](#5-citation)]

This is official code for our **BMVC 2022 paper**:<br>
[Title of Your Paper](Link)
<br>
 
![MaskSup Design](https://github.com/hasibzunair/masksup-segmentation/blob/master/media/pipeline.png?raw=true)

Summarize in 3-5 sentences your project here.

## 1. Specification of dependencies

This code requires Python YOUR_PYTHON_VERSION and CUDA YOUR_CUDA_VERSION. Create and activate the following conda envrionment.

```
conda update conda
conda env create -f environment.yml
conda activate myenv
```

## 2a. Training code

### Dataset details
We expect Dataset1 and Dataset2 datasets to have the following structure:
```
datasets/
|-- Dataset1/
|---- VOC2007/
|------ JPEGImages/
|------ Annotations/
|------ ImageSets/
......
|-- Dataset2/
|---- annotations/
|---- images/
|------ train2014/
|------ val2014/
...
```
Add any intructions for pre-processing data, to make it ready for training.

### Dataset1 training
```
python train.py --dataset Dataset1
```

### Dataset2 training
```
python train.py --dataset Dataset2
```

## 2b. Evaluation code

### Dataset1 eval
```
python eval.py --dataset Dataset1
```

### Dataset2 eval
```
python eval.py --dataset Dataset2
```

Refer to supplementary materials if any.

## 3. Pre-trained models

We provide pretrained models on [GitHub Releases](https://github.com/hasibzunair/masksup-segmentation/releases/tag/v0.1) for reproducibility. 
|Dataset      | Backbone  |   mIoU(%)  |   Download   |
|  ---------- | -------   |  ------ |  --------   |
| GLaS     |LeViT-UNet 384  |  76.06  | [download](https://github.com/hasibzunair/masksup-segmentation/releases/download/v0.1/masksupglas76.06iou.pth)   |
| Kvasir & CVC-ClinicDB     |LeViT-UNet 384 | 84.02  | [download](https://github.com/hasibzunair/masksup-segmentation/releases/download/v0.1/masksuppolyp84.02iou.pth)  |
| NYUDv2        |U-Net++ |  39.31  |  [download](https://github.com/hasibzunair/masksup-segmentation/releases/download/v0.1/masksupnyu39.31iou.pth)   |

## 4. Demo
Add demo details here.

## 5. Citation

If you use X in your research, please use the following BibTeX entry.

```bibtex
 @inproceedings{zunair2022masked,
    title={Masked Supervised Learning for Semantic Segmentation},
    author={Zunair, Hasib and Hamza, A Ben},
    booktitle={Proc. British Machine Vision Conference},
    year={2022}
  }
```

## Project Notes

<details><summary>Click to view</summary>
<br>

**[July 12, 2022]** Added this fancy drop down!
 
**[March 22, 2022]** I started making this template for my own reference. 

</details>

## Acknowledgements
Give credits to codebases you built on!


### Useful resources
* [Reproducibility Checklist](https://www.cs.mcgill.ca/~jpineau/ReproducibilityChecklist.pdf)
