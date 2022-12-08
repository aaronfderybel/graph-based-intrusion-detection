# Graph based modeling for intelligent monitoring.

Detecting malicious actions on a network with the use of artificial intelligence is called intelligent monitoring. To be more precise a number of standard attack techniques can be detected by collecting various information from the network.

Tabular data or "excel-like" data is the typical form datasets are stored in. Graph data is a different form and consists of a number of nodes that are connected through each other with edges. A simple example of a graph dataset is shown in the figure below. A social network such a facebook can keep track of friend connections and interests of different people through a graph.

![graph social network](assets/example_graph.PNG)

Graph data and the algorithms designed for this form of data has grown into a sub-domain of AI called graph neural networks. A very clear and visual introduction of graphs can be find here: [gentle introduction to graphs](https://distill.pub/2021/gnn-intro/)

In a similar fashion a graph can be constructed to contain information from a computer network to be able to detect malicious connections. The jupyter notebooks and scripts go through the example of converting an open-source dataset to graphs and applying a graph neural network.

* To understand how the code works go through the jupyter notebooks.
* To quickly try out different preprocessing and training options use the python scripts through the command line.

To run the scripts with the default options run the scripts `preprocess.py` and `train_graph.py` from terminal.

To show all the arguments of a script you can run from terminal:
```bash
python preprocess.py -h
```

To run the preprocessing script to make a test set with 40% of the data.
```bash
python preprocess.py --test-size 0.4
```


## install instructions

Install the basic libraries through pip
```bash
pip install -r requirements.txt
```

Install the pytorch and pytorch geometric libraries in order. Depending on your hardware setup and OS this can be quite different.
```bash
# pytorch installation see https://pytorch.org/get-started/locally/
# example for ubuntu with cuda 11.6 using pip below
pip install torch --extra-index-url https://download.pytorch.org/whl/cu116

# pytorch geometric installation see https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html
# example for ubuntu with cuda 11.6 and torch 11.3 using pip below
pip install pyg-lib torch-scatter torch-sparse torch-cluster torch-spline-conv torch-geometric -f https://data.pyg.org/whl/torch-1.13.0+cu116.html
```