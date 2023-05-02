Download Link: https://assignmentchef.com/product/solved-cpe202-lab-9-connected-graphs
<br>
<h1>Finding connected components</h1>

Finding connected components and graph coloring are important problems in computer science.  Connected components in an undirected graph give information about sets of vertices such that each pair of vertices has a path between them.

Implement algorithms based on <strong>Depth First Search</strong> to:

Determine the connected components of an undirected graph

An input file consists of one graph for testing.

<ul>

 <li>Each graph will represent an undirected graph.</li>

 <li>The first line contains a <strong>positive integer</strong> <strong><u>n</u></strong>, that is the number of vertices in the graph to be tested, where 1&lt;n&lt;200. Each vertex is represented by a number from 1 to n</li>

 <li>The second line is the number of edges, call this number <strong>e</strong>.</li>

 <li>This is followed by <strong>e</strong> lines each containing a pair of integers each integer between 1 and n separated by a</li>

</ul>

space that represents an edge between the vertices represented by the numbers.

Implement the following functions

─ <strong>def  __init__ (self, filename</strong>): reads in the specification of a graph and creates a graph using an adjacency list representation.  You may assume the graph is not empty and is a correct specification.

E.g. each edge is represented by a pair of vertices between 1 and n.  Note that the graph is <strong>not directed</strong> so each edge specified in the input file should appear on the adjacency list of each vertex of the two vertices associated with the edge.

─ <strong>def conn_components (self): </strong>returns a list of lists.  For example, if there are three connected components then you will return a list of three lists.  The order of the sub-lists is not important.  However each sub-list will contain the vertices (in ascending order) in the connected component represented by that list.  Each vertex is represented by an integer from 1 to n.   If a vertex has no edges it will be in a connected component containing only itself.  <strong> </strong>

<strong>SUBMISSION </strong>

Upload a file to PolyLearn, <strong>my_graph.py</strong> containing a class <strong>MyGraph</strong>, that contains your new graph class including functions that determine the connected components, <strong>conn_components (self)</strong>.




<strong>Examples: </strong>

<strong>Input: </strong>

9

8

1 2

1 3

1 4

1 5

<ul>

 <li>7</li>

 <li>9</li>

</ul>

9 8

<ul>

 <li>6</li>

</ul>

<strong> </strong>

<ul>

 <li><strong>is number of vertices and 8 is number of edges. If the graph created is g1, then </strong></li>

</ul>

<strong>g1.conn_components() returns: </strong><strong>[[1, 2, 3, 4, 5], [6, 7, 8, 9]]</strong>

<strong> </strong>

<strong>Input: </strong>

8

6

<ul>

 <li>2</li>

 <li>3</li>

 <li>1</li>

 <li>6</li>

</ul>

4 7

4 8

<strong> </strong>

<strong>8 is number of vertices and 6 is number of edges. </strong>

<strong>In this graph based on 8 vertices 5 is not connected to any other vertices and has no edges, therefore it is a sublist contains itself. </strong>

<strong> </strong>

<strong>If the graph created is g2, then  </strong>

<strong>g2.conn_components() returns: </strong><strong>[[1, 2, 3], [4, 6, 7, 8] [5]]</strong>

<strong> </strong>