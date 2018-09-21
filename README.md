# NAMVH
This repository provides the implementation of *NAMVH* as described in the papers:

> Nonlinear Asymmetric Multi-Valued Hashing<br>
> Cheng Da, Gaofeng Meng, Shiming Xiang, Kun Ding, Shibiao Xu, Qing Yang, and Chunhong Pan<br>
> TPAMI, 2018.<br>


Meanwhile, this repository also provides the implementation of *AMVH* as described in the papers:

> AMVH: Asymmetric Multi-Valued Hashing<br>
> Cheng Da, Shibiao Xu, Kun Ding, Gaofeng Meng, Shiming Xiang, Chunhong Pan<br>
> CVPR, 2017.<br>

# Prerequisites

Linux 16.04.5
NVIDIA GPU + CUDA-8.0 and corresponding CuDNN

Caffe

Matlab 2015b

# Installation Guide

You need to compile the modified Caffe library in this repository. You can consult the generic [Caffe installation guide](http://caffe.berkeleyvision.org/installation.html).

When the dependencies of Caffe are installed, try:

```
make
```

If there are no error messages, then you can compile and install the matlab wrappers:
```
make matcaffe
```

# Usage 
run AMVH for AMVH: Asymmetric Multi-Valued Hashing on ESP-GAME

```
cd NAMVH
matlab -r -nodesktop run_AMVH on ESP-GAME with 8-bit codes.
```

#### results
    maps =

    0.4362    0.4906
    0.4953    0.5190


run NAMVH for Nonlinear Asymmetric Multi-Valued Hashing on ESP-GAME with 8-bit codes.

```
cd NAMVH
matlab -r -nodesktop run_NAMVH
```

#### results
    maps =

    0.4822    0.5045
    0.5208    0.5599

	> noted: maps = <br>
	        AMVH_bin  AMVH_real
					  AMVH_mul
# Datasets
We provide ESP-GAME dataset [./data](https://github.com/dcfucheng/NAMVH/tree/master/data) to test our codes.

### Citing
If you find *NAMVH* and *AMVH* useful in your research, please consider citing the following paper:

	@ARTICLE{8451950, 
	author={C. Da and G. Meng and S. Xiang and K. Ding and S. Xu and Q. Yang and C. Pan}, 
	journal={IEEE Transactions on Pattern Analysis and Machine Intelligence}, 
	title={Nonlinear Asymmetric Multi-Valued Hashing}, 
	year={2018}, 
	volume={PP}, 
	number={1}, 
	pages={1-1}, 
	doi={10.1109/TPAMI.2018.2867866}, 
	ISSN={0162-8828}, 
	}
	
	@inproceedings{DBLP:conf/cvpr/DaXDMXP17,
	author    = {Cheng Da and
               Shibiao Xu and
               Kun Ding and
               Gaofeng Meng and
               Shiming Xiang and
               Chunhong Pan},
	title     = {{AMVH:} Asymmetric Multi-Valued hashing},
	booktitle = {{IEEE} Conference on Computer Vision and Pattern Recognition,{CVPR}},
	pages     = {898--906},
	year      = {2017},
	url       = {https://doi.org/10.1109/CVPR.2017.102},
	doi       = {10.1109/CVPR.2017.102},
	}
	
	
	