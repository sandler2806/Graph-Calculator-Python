<p align = "center"><img src = "https://user-images.githubusercontent.com/74304423/146420213-3c28708b-2a6c-479f-bb83-84ea747c3944.png">  </p>

<p>
<h2>  Project review</h2>
Graph calculator is a simple program that can create, load(via JSON file) , and edit directed weighted graphs. After receiving/loading a graph from a JSON file it can be used as the basis for many graph operations, such as finding the shortest path between two nodes, finding the center, etc...<br>
The manipulated graph can be saved to json file.
</p>

<h2> Algorithms </h2>


 <ul>
  
  <li> <strong>Shortest path: </strong>We call Dijkstra's algorithm on the source node, fetch the parents array it returns, and use it to calculate the path to the destination vertex Then, using backtracking we construct the path between these two nodes. </li>
  <li> <strong> Center: </strong>The implementation is rather simple, we first compute the eccentricity of each node <a href="https://en.wikipedia.org/wiki/Distance_(graph_theory)">(eccentricity:wikipedia) </a> using Dijkstra's algorithm on each vertex and taking the max distance. then, we  pick the vertex with the smallest eccentricy as the center</li>
  
  <li> <strong> Tsp-Traveling salesmen problem: </strong> We start from some random node from the list, perform the Dijkstra algorithm, and travel to the closest Unvisited node from the list, we keep doing that until we reached all the nodes from the list. following this method will yield us a valid path, albeit not necessarily the shortest. we repeat this process for each node in the list, each time picking another vertex as a starting point. in the end we return the shortest path we've found</li>  

 <h3> DIjkstra's shortest path algorithm</h3>
 <p>
  Dijkstra's algorithm played a major part in our work, being part of every algorithm. After our first implementation of the algorithm (using regular priority queue) proved to be too slow for our purposes, we implemented it again using python's min heap Queue library - heapq.
Using the new implementation and after little bit of profiling, we managed to  greatly improve our running time.
 </p>


 <h2> UML diagram </h2>
 <br>
 <p align = "center"><img src = "https://user-images.githubusercontent.com/74304423/146753790-d87e99b6-1ebc-4b13-848d-61780a15cbf5.jpg">  </p>
 
 <h2> How to run the project </h2>
 
 <h2> Visual representation </h2>