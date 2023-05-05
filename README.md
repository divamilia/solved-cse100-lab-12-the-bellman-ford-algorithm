Download Link: https://assignmentchef.com/product/solved-cse100-lab-12-the-bellman-ford-algorithm
<br>
<strong>The Bellman-Ford Algorithm</strong>

In this assignment, you are asked to implement the Bellman-Ford Algorithm which solves the single-source shortest-paths problem. Specifically, you are given as input a directed graph <em>G </em>= (<em>V,E</em>) with weight <em>w</em>(<em>u,v</em>) on each edge (<em>u,v</em>) ∈ <em>E </em>along with a source vertex <em>s </em>∈ <em>V </em>. Edges may have negative weights.

<strong>Input </strong>The input has the following format. There are two integers on the first line. The first integer represents the number of vertices, |<em>V </em>|. The second integer is the number of edges, |<em>E</em>|. Vertices are indexed by 0<em>,</em>1<em>,…,</em>|<em>V </em>| − 1. Each of the following |<em>E</em>| lines has three integers <em>u,v,w</em>(<em>u,v</em>) , which represent an edge (<em>u,v</em>) with weight <em>w</em>(<em>u,v</em>). Vertex 0 is the source vertex.

<strong>Output      </strong>The output falls into two possible cases.

Case (i): There is no negative-weight cycle reachable from <em>s</em>. In this case, you must output TRUE on the first line, followed by the shortest distance from <em>s </em>to each vertex in the graph. More precisely, you must output TRUE, <em>δ</em>(0<em>,</em>0), <em>δ</em>(0<em>,</em>1), <em>…</em>, <em>δ</em>(0<em>,</em>|<em>V </em>| − 1), one per line. Recall that <em>δ</em>(<em>u,v</em>) denotes the shortest distance from <em>u </em>to <em>v</em>. If a vertex <em>v </em>is not reachable, output INFINITY in place of <em>δ</em>(0<em>,v</em>).

Case (ii): There is a negative-weight cycle reachable from <em>s</em>. You must output FALSE.

<strong>Examples of input and output</strong>

<a href="#_Toc2093">Input                                                           1</a>

<a href="#_Toc2094">6 10                                                             </a>

<a href="#_Toc2095">0 1 61 2 51 3 -41 4 82 1                                                     2</a>

<a href="#_Toc2096">3 0                                                             2</a>




3 2 7

<ul>

 <li>4 9</li>

 <li>0 7</li>

 <li>2 5</li>

</ul>

Output 1

TRUE

0

6

9

2

11

INFINITY

<h1><a name="_Toc2093"></a>Input 2</h1>

<h1><a name="_Toc2094"></a>6 11</h1>

<h1><a name="_Toc2095"></a>0 1 6</h1>

1 2 5

1 3 -4

<ul>

 <li>4 8</li>

 <li>1 -2</li>

</ul>

<h1><a name="_Toc2096"></a>3 0 2</h1>

3 2 7

3 4 9

<ul>

 <li>5 -14</li>

 <li>0 7</li>

 <li>2 5</li>

</ul>

Output 2

FALSE

Note that every line is followed by an enter key.

See the lab guidelines for submission/grading, etc., which can be found in Files/Labs.