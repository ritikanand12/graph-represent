Graph Implementation Using Adjacency List in C

This project demonstrates how to implement a Graph using an Adjacency List in C programming language.

The graph is represented using linked lists, where each vertex maintains a list of its adjacent vertices.

📌 Description

In this program:

A graph of 5 vertices is created.

The adjacency list is implemented using a linked list.

Edges are added using the addEdge() function.

The graph is displayed using the display() function.

This implementation represents a directed graph.

🧠 What is an Adjacency List?

An adjacency list represents a graph as:

An array of linked lists.

Each index represents a vertex.

Each linked list contains adjacent vertices.

It is more memory-efficient than an adjacency matrix for sparse graphs.

📂 Data Structures Used
🔹 Node Structure
struct Node {
    int vertex;
    struct Node* next;
};
🔹 Adjacency List Array
struct Node* adj[5];

adj[i] stores the head of the linked list for vertex i.

🔁 Functions Explained
➤ addEdge(int u, int v)

Creates a new node.

Inserts vertex v at the beginning of the linked list of vertex u.

➤ display()

Traverses each linked list.

Prints all adjacent vertices for every vertex.

🖥️ Graph Created in Program

Edges added:

0 → 1
0 → 2
1 → 3
3 → 4

Graph Representation:

0 → 2 → 1
1 → 3
2 → NULL
3 → 4
4 → NULL

(Note: Order depends on insertion at head.)

▶️ Sample Output
Vertex 0: 2 -> 1 -> NULL
Vertex 1: 3 -> NULL
Vertex 2: NULL
Vertex 3: 4 -> NULL
Vertex 4: NULL
⚙️ How to Compile and Run
1️⃣ Compile
gcc adjacency_list.c -o adjacency_list
2️⃣ Run
./adjacency_list
⏱️ Time & Space Complexity
Time Complexity:

Adding an edge: O(1)

Displaying graph: O(V + E)

Space Complexity:

O(V + E)

Where:

V = Number of vertices

E = Number of edges

📚 Concepts Covered

Graph Representation

Adjacency List

Linked List

Dynamic Memory Allocation

Directed Graph

⚠️ Limitations

Number of vertices is fixed (5).

No memory deallocation (free() not used).

No user input handling.

Only directed edges are implemented.

🚀 Possible Improvements

Make number of vertices dynamic.

Add support for undirected graphs.

Implement BFS and DFS using adjacency list.

Add edge deletion.

Free allocated memory.

👨‍💻 Author

Ritik Chauhan

If you want, I can also provide:

Undirected graph version

BFS/DFS using adjacency list

Weighted graph implementation

Menu-driven graph program
