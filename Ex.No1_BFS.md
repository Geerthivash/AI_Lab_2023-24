# Ex.No: 1  Implementation of Breadth First Search 
### DATE: 07 - 03 - 25                                                                      
### REGISTER NUMBER : 212223060067
### AIM: 
To write a python program to implement Breadth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function bfs and take the set “visited” is empty and “queue” is empty
4. Search start with initial node and add the node to visited and queue.
5. For each neighbor node, check node is not in visited then add node to visited and queue list.
6.  Creating loop to print the visited node.
7.   Call the bfs function by passing arguments visited, graph and starting node.
8.   Stop the program.
### Program:

```
from collections import deque


def bfs(graph, start):
    while queue:
        vertex = queue.popleft()
        bfs_order.append(vertex)
        for neighbor in graph[vertex]:
            if neighbor not in visited:
                visited.add(neighbor)
                queue.append(neighbor)
     return bfs_order

graph = {
    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []
}

start_vertex = 'A'
order = bfs(graph, start_vertex)
print("BFS Order:", order)

```

### Output:

![image](https://github.com/user-attachments/assets/6771e719-3d14-4c17-98f2-a0c76d2fd25f)


### Result:
Thus the breadth first search order was found sucessfully.
