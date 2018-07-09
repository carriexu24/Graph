# Graph
A directed un-weighted in your Graph class implementation.

## Examples


```
from graph import *

# create an empty node
node = Node({})

# create a graph with a list of nodes
node_list = []
node_list.append(Node({'A':['B','C']}))
node_list.append(Node({'B':['C','D']}))
node_list.append(Node({'C':['D']}))
node_list.append(Node({'D':['C']}))
Graph(node_list)

# add nodes to a graph
g = Graph()
for node in node_list:
    g.add(node)

# find paths
g.find_path_dfs("A", "D")
g.find_all_paths("A", "D")
g.find_shortest_path("A", "D")

# check if there is a path between nodes
g.has_route("C", "B")
```
