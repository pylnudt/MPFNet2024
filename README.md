
### Source Code for Papers:

`MPFNet: A Radar Extrapolation Network Based on Multi-product Fusion `

#### * Installing Libraries:
```shell
pip3 install -r requirements.txt --extra-index-url https://download.pytorch.org/whl/cu113
```
### Hyperparameters:
See models/config.py

###  Running(there are three type of model variants for different combinations of radar product inputs):
```shell
python -m torch.distributed.launch --nproc_per_node=4 main_single.py
python -m torch.distributed.launch --nproc_per_node=4 main_double.py
python -m torch.distributed.launch --nproc_per_node=4 main_tri.py
```
