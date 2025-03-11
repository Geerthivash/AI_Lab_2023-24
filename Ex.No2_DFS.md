# Ex.No: 2  Implementation of Depth First Search
### DATE: 07 - 03 - 25                                                                        
### REGISTER NUMBER : 212223060067
### AIM: 
To write a python program to implement Depth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the dfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.
### Program:



```

# Python program to implement Depth First Search (DFS)
# Graph represented as an adjacency list

def dfs(graph, node, visited=None):
    if visited is None:
        visited = set()  # Using a set for O(1) membership checks
    if node not in visited:
        print(node, end=" ")  # Process the node (here, we print it)
        visited.add(node)
        for neighbor in graph[node]:
            dfs(graph, neighbor, visited)
    return visited

# Example graph: vertices as numbers
graph = {
    1: [2, 3],
    2: [4, 5],
    3: [6],
    4: [],
    5: [6],
    6: []
}

# Starting DFS from node 1 (experiment may specify a different start)
print("DFS Order:")
dfs(graph, 1)


```

### Output:

![image](https://github.com/user-attachments/assets/03715b72-bba0-48f0-a930-8b3f244d3cc4)


### Result:
Thus the depth first search order was found sucessfully.
