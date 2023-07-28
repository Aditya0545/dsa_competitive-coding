# Connected Components in Graph

The graph can have different components which may not be connected as shown in image below, But they need to be counted when we are traversing a graph.  

![Connected Components in Graph](https://media.geeksforgeeks.org/wp-content/uploads/20200421194558/Count-of-Connected-Components.png)  


To count such nodes when traversing, Create another visited array of nodes and from that array, Call traversing algorithms like DFS or BFS.

Representation:
```cpp
vector<int> vis(n+1, 0);
for(int i=0;i<n;i++){
    if(vis[i]!=0){
        traversal_algo(i);
    }
}
```