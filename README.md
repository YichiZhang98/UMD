# UMD

The official repo of "[Uncovering Modality Discrepancy and Generalization Illusion for General-Purpose 3D Medical Segmentation](https://arxiv.org/pdf/2602.07643)".


## 🔬 Background & Motivation
The recent emergence of 3D medical foundation models has marked a significant milestone toward general-purpose medical image segmentation. However, a critical examination of current validation protocols reveals several pitfalls that obscure the true limits of these models. Most existing evaluations are heavily concentrated on structural imaging (CT and MRI), while functional imaging domain (e.g., PET) remain largely untested. Current evaluation protocols typically measure a model's performance across different datasets ang targets. This neglects the Modality Discrepancy that exists when the anatomy remains constant but the imaging physics changes.

![image](https://github.com/YichiZhang98/UMD/blob/main/UMD.png)


## 🛡️ The UMD Solution

UMD is a large-scale, multi-modal benchmark dataset specifically designed to quantify Modality Discrepancy and expose the Generalization Illusion in general-purpose 3D segmentation models. UMD dataset comprising 490 whole-body PET/CT and 464 whole-body PET/MRI scans for segmentation of 13 paired target organs. By providing paired PET/CT and PET/MRI scans from the same individuals, UMD allows for the first rigorous intra-subject comparative analysis. It serves as a stress test to determine whether a model's anatomical knowledge is truly modality-agnostic or merely an artifact of structural imaging patterns.

## 📈 Key Findings

Our analysis reveals that current foundation models are not truly general- purpose, exhibiting a systemic structural bias that leads to catastrophic perfor- mance failure in functional domains. Despite high reported benchmarks, these models remain limited generalization ability in unseen data distributions. Please refer to [the paper](https://arxiv.org/pdf/2602.07643) for more details.

## 📂 Data Structure & Usage

Coming soon.


## 🖋️ Citation

If you find this repository helpful, please consider citing:
```
@article{zhang2026uncovering,
  title={Uncovering Modality Discrepancy and Generalization Illusion for General-Purpose 3D Medical Segmentation},
  author={Zhang, Yichi and Xiao, Feiyang and Xue, Le and Zhang, Wenbo and Feng, Gang and Zheng, Chenguang and Qi, Yuan and Cheng, Yuan and Hu, Zixin},
  journal={arXiv preprint arXiv:2602.07643},
  year={2026}
}
```
