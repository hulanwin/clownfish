# Clownfish
Edge and Cloud Symbiosis for Video Stream Analytics.

If you find our paper or code useful to your research, please do cite our article.
```bib
@inproceedings{nigade2020clownfish,
  title={{Clownfish}: Edge and Cloud Symbiosis for Video Stream Analytics,
  author={Vinod Nigade and Lin Wang and Henri Bal},
  booktitle={{ACM/IEEE} Symposium on Edge Computing ({SEC})},
  year={2020}
}
```

# Getting started

Clone this repository and checkout submodules.
```
$ git submodule update --init --recursive
```

# How to use

This repository contains three submodules. 

1. [clownfish-3D-models](https://github.com/vnigade/clownfish-3D-models/tree/16c8c2e101af890e9bbf40842c164c912cd9ae91)

This submodule contains code to train (fine-tune) models such as `3D-ResNets`, `SimiNet`, `EarlyDiscard (3D-MobileNet)`, etc. on the `PKU-MMD` action recognition dataset. It also contains scripts to dump prediction scores (results) in JSON files for videos using a sliding window scheme.

2. [clownfish-analysis](https://github.com/vnigade/clownfish-analysis/tree/fbb472d13c5d2c538f376f33e952ffdeb9ec4023)

This submodule contains scripts to analyze the accuracy of fusion for different `filter intervals` and `lag` values. It uses the prediction scores (results) of edge and cloud models which are dumped using the above-mentioned submodule (clownfish-3D-models).

3. [clownfish-proto](https://github.com/vnigade/clownfish-proto/tree/1a42ab05b070b837895b426a980bf04cb3f9052c)

This submodule implements the Clownfish prototype. It can be used to run Clownfish components on an edge and cloud node, for action recognition task on the `PKU-MMD` dataset.


Please refer to the individual `README` files for more details.



