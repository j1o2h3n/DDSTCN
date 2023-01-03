# DDSTGCN

Y. Sun, X. Jiang, Y. Hu, F. Duan, K. Guo, B. Wang, J. Gao, B. Yin, "[Dual Dynamic Spatial-Temporal Graph Convolution Network for Traffic Prediction](https://ieeexplore.ieee.org/document/9912360)," in IEEE Transactions on Intelligent Transportation Systems, vol. 23, no. 12, pp. 23680-23693, Dec. 2022, doi: 10.1109/TITS.2022.3208943.

<p align="center">
  <img width="826" height="303" src=./fig/picture.jpg>
</p>


## Requirements

- python 3
- numpy
- torch

## Train Commands

```
python train.py

OR

python train.py --data=data/METR-LA --adjdata=data/METR-LA/adj_mx.pkl --in_dim=2 --num_nodes=207
```

To run different datasets, you need to modify the relevant parameters of the dataset, including '--data', '--adjdata', '--in_dim' and '--num_nodes'. The default is METR-LA dataset.


### Dataset

|  Dataset |     --data    |           --adjdata          | --in_dim | --num_nodes |
|:--------:|:-------------:|:----------------------------:|:--------:|:-----------:|
|  METR-LA |  data/METR-LA |    data/METR-LA/adj_mx.pkl   |     2    |     207     |
| PEMS-BAY | data/PEMS-BAY | data/PEMS-BAY/adj_mx_bay.pkl |     2    |     325     |
|  PEMS03  |  data/PEMS03  |  data/PEMS03/adj_pems03.pkl  |     1    |     358     |
|  PEMS04  |  data/PEMS04  |  data/PEMS04/adj_pems04.pkl  |     1    |     307     |
|  PEMS07  |  data/PEMS07  |  data/PEMS07/adj_pems07.pkl  |     1    |     883     |
|  PEMS08  |  data/PEMS08  |  data/PEMS08/adj_pems08.pkl  |     1    |     170     |

Dataset URL: https://drive.google.com/drive/folders/1uoY8ROQU73BqWyl566ZNdRBOOTM4T2DS?usp=sharing


## License
This repo is under [MIT license](LICENSE).



## Citation
If you find this repo useful in your research, please cite the following in your manuscript:

```bibtex
@ARTICLE{sun2022dual,
author={Sun, Yanfeng and Jiang, Xiangheng and Hu, Yongli and Duan, Fuqing and Guo, Kan and Wang, Boyue and Gao, Junbin and Yin, Baocai},
   journal={IEEE Transactions on Intelligent Transportation Systems},
   title={Dual Dynamic Spatial-Temporal Graph Convolution Network for Traffic Prediction},
   year={2022},
   volume={23},
   number={12},
   pages={23680-23693},
   publisher={IEEE},
   doi={10.1109/TITS.2022.3208943}
}
```
