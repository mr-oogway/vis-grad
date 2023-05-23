# visgrad

A computational graph visualizer of a DL model. It has the values and grads in each nodes and can perform backpropagation to update the parameters.

Uses an object that wraps the numpy.array into a node such that it has also its parents that the tensor is coming from, the operator used and also the gradients. A DAG is made using these nodes, then using `graphviz` library the graph is rendered.