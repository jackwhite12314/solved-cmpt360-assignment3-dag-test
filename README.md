Download Link: https://assignmentchef.com/product/solved-cmpt360-assignment3-dag-test
<br>
<h1>DAG TEST</h1>

Given an edge list of a directed graph, the task is to test whether the graph is acyclic or not.

<strong>Input:</strong>

The input is in ‘TestGraph.txt’. Each line contains the source and target string separated by ‘,’. The ‘END’denotes the end of the edge list. The following input contains two graphs. <strong>Sample input:</strong>

2,4

4,3 4,6 END

2,3

3,4

4,2

END

<strong>Output:</strong>

Each line of the output contains True or False, depending on whether the graph is a DAG or not.

<strong>Sample output:</strong>

TRUE

FALSE

<strong>Instructions:</strong>

Edit the given code TestGraph.java to complete the assignment. Do not edit the part which is READ ONLY. Submit TestGraph.java in Moodle. Note that you need to carefully read the given print function to understand how you can traverse a graph with the given graph data structure.

<h1>B. Constrained Edit distance</h1>

In this question we are trying to solve the edit distance problem from the book (by insertion, deletion, substitution), but avoiding same operation applied consecutively.

For example, if the input is (APPLE,MAPLE), then the following transformation is invalid: APPLE (deletion) APLE (deletion) PLE (insertion) MPLE (insertion) MAPLE. There is another invalid transformation with cost 2: APPLE (substitution) MPPLE (substitution) MAPLE.

A valid sequence would be APPLE (deletion) APLE (insertion) AMPLE (deletion) MPLE (insertion) MAPLE. However, this is not a minimum cost solution. There is another valid transformation with cost 3: APPLE (substitution) MPPLE (deletion) MPLE (insertion) MAPLE.

Consider another example (GO,ALGORITHM). In this case there is no valid solution. Because, you have to perform at least 7 insertions, so there is no way you can avoid consecutive insertions.

Modify the recurrence provided in the book for the edit distance algorithm. For more input output see the official page in piazza.

<strong>Input:</strong>

The input is in ‘edit.txt’. Each line contains the source and target string separated by ‘,’. <strong>Sample input:</strong>

APPLE,MAPLE

GO,ALGORITHM

<strong>Output:</strong>

Each line of the output contains the cost, which is the edit distance cost for the corresponding input. If there is no valid solution, then the output is -1. <strong>Sample output:</strong>

2

-1

<strong>Instructions:</strong>

Edit the given code Edit.java to complete the assignment. Do not edit the part which is READ ONLY. Submit Edit.java in Moodle.