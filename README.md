# CS241PA5
Strongly Connected Graphs

Project 5 – Strongly Connected Components

1.	Requirements: 
This project involved determining the strongly connected components of a directed graph.  Given an input graph file, the program will construct the graph and print out the adjacency lists. The project required creating a class that extended the provided DfsGraph.java class and overriding the depth-first search methods to implement the strongly connected components pseudocode algorithm described on the course site. The program will then output the vertices in each strongly connected component. The program will utilize the test case graph7.txt and graph8.txt provided also on the course site.

2.	Method:
	The project utilized the source code provided which included the files DfsGraph.java, Edge.java, Graph.java, and Vertex.java. Following the strongly connected components algorithm outlined on the course site to compute the strongly connected components given a directed graph. 

3.	Implementation:
The StronglyConnected.java class was implemented to extend the DfsGraph.java class and included a main method to execute the program. This class also included the overridden preVisit and postVisit methods. By following the algorithm, it was necessary to implement a Boolean start value that would indicate whether the depth-first search was being run at the beginning or at the end of the algorithm. Given a directed graph g, the program performed a persistent depth-first search on g. It would then push each vertex v into a stack. The program would then construct a graph h, which was a copy of g with its edges reversed. It would then perform a persistent depth-first search on h, visiting the vertices using the stack in LIFO order. Whenever a new search was initiated, it would indicate a new strongly connected component within the graph. Finally, the main method would then output the strongly-connected components and its vertices. 

4.	Testing:
To ensure that the program correctly identified the strongly connected components of a directed graph, the program utilized graph7.txt as a test case. The results of the output of the strongly connected components were then compared to the example on the course site and verified. Once this was accomplished, the program utilized graph8.txt as the final test case. 

5.	Findings: 
	From this project, I learned more about overriding methods that were designed for modularity. I also had to think about why I was getting an empty stack exception even after following the pseudocode algorithm and figure out a way to maintain the integrity of the algorithm while making the code work.
