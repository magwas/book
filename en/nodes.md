###Nodes, metagroups, organising nodes

The Node is an abstraction of the model. The group is a type of node. The group of groups - called metagroup - is also a type of it.
Nodes are the same notion as it is used in graph theory. So the nodes can have parents and children, they define a subtree, and the whole formal structure itself is a tree with exactly one root node. We use “up” to signify the direction towards the root node.
Nodes can capture different organisations of people: local, state or federal governments, clubs, movements, even companies (though that would be rather socialistic to do in the formal structure).
Nodes can have properties, eligibility requirements, rules and officials. 
Metagroups however cannot have direct members, just groups or other metagroups. The number of members in a metagroup must be more than one, and there is also an upper limit, e.g. 90.
When a node splits, the descendant nodes will both be members of the original parent node if the eligibility requirement is the same. Otherwise a new metagroup will form in the place of the node, and the descendant nodes will belong to that.
An “organising node” is a node which is the top node of a subtree with the same eligibility requirement. The root node is an organising node.
Nodes can choose (using the decision making procedures described below) to move within the structure. In order to keep the tree balanced, movements are restricted to those who do not cause a group to be closer to organizing nodes than the closest group before the move.
A node automatically inherits from its parent metagroup the eligibility requirement and all rules applicable to the group, if not overridden locally. 

