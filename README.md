# TorchGT
A pytorch implementation of TorchGT.

Model implementation is based on "Do Transformers Really Perform Bad for Graph Representation" (NeurIPS'21) [[paper]](https://proceedings.neurips.cc/paper/2021/hash/f1c1592588411002af340cbaedd6fc33-Abstract.html) [[github]](https://github.com/microsoft/Graphormer). 


## Run the code  
Environment: gt

### Graph-level
```bash
torchrun --nproc_per_node=4 main_sp_graph_level.py --dataset Malnet
```
 
### Node-level
Use preprocess_data.py for data downloading and preprocessing

```bash
torchrun --nproc_per_node=4 --master_port 1234 main_sp_node_level.py --dataset ogbn-products
```






