# Graph based modeling for intelligent monitoring.

Detecting malicious actions on a network with the use of artificial intelligence is called intelligent monitoring. To be more precise a number of standard attack techniques can be detected by collecting various information from the network.

Tabular data or "excel-like" data is the typical form datasets are stored in. Graph data is a different form and consists of a number of nodes that are connected through each other with edges. A simple example of a graph dataset is shown in the figure below. A social network such a facebook can keep track of friend connections and interests of different people through a graph.

![graph social network](assets/example_graph.PNG)

Graph data and the algorithms designed for this form of data has grown into a sub-domain of AI called graph neural networks. A very clear and visual introduction of graphs can be find here: [gentle introduction to graphs](https://distill.pub/2021/gnn-intro/)

In a similar fashion a graph can be constructed to contain information from a computer network to be able to detect malicious connections. The jupyter notebooks and scripts go through the example of converting an open-source dataset to graphs and applying a graph neural network.

* To understand how the code works go through the jupyter notebooks.
* To quickly try out different preprocessing and training options use the python scripts through the command line.

To download and preprocess the example dataset with default arguments run from terminal: `python preprocess.py`.
If you would like to change some options in the preprocessing run from terminal: `python preprocess.py -h`
This shows all the possible arguments that can be adapted and their meaning. The script for training and evaluating graphs is constructed in a similar way.


## install instructions

Install the basic libraries through pip
```bash
pip install -r requirements.txt
```

Install the pytorch and pytorch geometric libraries in order.
Depending on your hardware setup and OS this can be quite different.
[Pytorch install](https://pytorch.org/get-started/locally/)
[Pytorch geo install](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html)
