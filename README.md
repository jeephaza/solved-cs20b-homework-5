Download Link: https://assignmentchef.com/product/solved-cs20b-homework-5
<br>
<ol>

 <li>Answer the questions below about the following tree, using the letters that label the nodes:

  <ul>

   <li>Which node is the root?</li>

   <li> Which node is the parent of F?</li>

   <li>Which node(s) are the children of H?</li>

   <li>Which node(s) are the ancestors of M?</li>

   <li> Which node(s) are the descendants of T?</li>

   <li> Which node(s) are the siblings of S? And of H?</li>

   <li>What is the height of the tree?</li>

   <li> Write the order in which the nodes are visited by a breadthfirst traversal. Use the following format when specifying the order: [node1 node2 … nodeN] Write the order in which the nodes are visited by a depthfirst traversal. Use the following format when specifying the order: [node1 node2 … nodeN]</li>

  </ul></li>

 <li>Answer the following questions about the binary search tree (in Figure 1).

  <ul>

   <li> What is the height of the tree?</li>

  </ul></li>

</ol>

Figure 1: A binary search tree

<ul>

 <li> Which nodes are on level 3?</li>

 <li> Which levels have the maximum number of nodes that they could contain?</li>

 <li>What is the maximum height of a binary search tree containing these nodes (counting level 0 as well)?</li>

 <li> What is the minimum height of a binary search tree containing these nodes (counting level 0 as well)?</li>

 <li> What is the order in which nodes are visited by a preorder traversal?</li>

 <li>What is the order in which nodes are visited by an inorder traversal?</li>

 <li> What is the order in which nodes are visited by a postorder traversal?</li>

 <li> What is the order in which nodes are visited by a depthfirst traversal?</li>

 <li> What is the order in which nodes are visited by a breadthfirst traversal?</li>

</ul>

<ol start="3">

 <li><strong>(Hashing from Chapter 8) </strong>Critique the following hash functions for a domain consisting of people with attributes <em>firstName</em>, <em>lastName</em>, <em>number </em>(used to resolve identical first and last names, e.g., “John Smith 0,” “John Smith 1,” etc.), and <em>age</em>. The names are of class String and the other two attributes are of type int.</li>

</ol>

<ul>

 <li>hash function returns (<em>age</em>)<sup>2</sup></li>

 <li>hash function returns (<em>age</em>)<sup>2 </sup>+ lastName.hashCode()</li>

 <li>hash function returns lastName.hashCode() + firstName.hashCode()</li>

 <li>hash function returns lastName.hashCode() + firstName.hashCode() + number</li>

</ul>

Note: answer the question in terms of how good the hashcode is for avoiding collisions (different entries having the same hashcode) and uniquely identifyng the objects.

<ol start="4">

 <li>(5 points) <strong>(Hashing from Chapter 8) </strong>Critique the following code which is intended to print out whether or not a key value <em>k</em>1 is used in a map named relationships:</li>

</ol>

1 if (relationships.get(k1) != null)

2

3                                                       System.out.println(“yes it does”);

4

5 else

6

7                                                         System.out.println(“no it does not”);

Now rewrite the code so that it works correctly

<ol start="5">

 <li>(10 points) <strong>(Graphs) </strong>Use the following description of an <strong>undirected graph </strong>for Questions a) and b) below:</li>

</ol>

EmployeeGraph = (V, E)

V(EmployeeGraph) = {Susan, Darlene, Mike, Fred, John, Sander, Lance, Jean, Brent, Fran}

E(EmployeeGraph) = {(Susan, Darlene), (Fred, Brent), (Sander, Susan), (Lance, Fran),

(Sander, Fran), (Fran, John), (Lance, Jean), (Jean, Susan), (Mike, Darlene), (Brent, Lance), (Susan, John)}

<ul>

 <li>Draw a picture of EmployeeGraph (draw it the way graphs look like – see the book or slides)</li>

 <li>Which one of the following phrases best describes the relationship represented by the edges between the vertices in EmployeeGraph and <strong>why</strong>?

  <ol>

   <li>“works for”</li>

   <li>“is the supervisor of ”</li>

  </ol></li>

</ul>

<ul>

 <li>“is senior to” iv. “works with”</li>

</ul>

<ol start="6">

 <li>(10 points) <strong>(Graphs) </strong>Draw the adjacency matrix for the graph in Figure 2. Store the vertices in alphabetical order.</li>

</ol>

<h1>1           Programming exercises</h1>

Please do these with your partner. The assignments are not precisely defined (as in the real-world) and you will have to figure out the details. You will need to

Figure 2: Graph example

show the concepts you learned in this class (OOP design) as much as possible. You will present your solution to the class in the final class of the semester. You will run your code and demonstrate how it works and then we will discuss the structure of your solution. I will ask each of you to write a report on your partner describing how much your partner contributed to this homework. Make sure you comment your code.

<h2>1.1         Problem 1: Logical Circuits</h2>

In this assignment using Java’s OOP design you need to represent the following logic gates: AND, OR, NOT and XOR. The basic functionality of your code should be the following:

<ol>

 <li>For each gate, given some inputs, get the calculated output. For example (this is pseudocode): AND(True, True) should give me True, XOR(True, False) should give me True. Make the application that makes sure <strong>each </strong>of your gate operates correctly with all combinations of binary inputs.</li>

 <li>(Bonus for A+) <strong>Go for the glory! </strong>This one is a bit more complicated but fun. Given a logic circuit calculate the output of the circuit. For example, for the circuit in Figure 3 and inputs A = TRUE, B = FALSE, C = FALSE, D = TRUE the circuit outputs FALSE. Don’t try to solve everything. Just make a solution for these simpler examples. Use the circuit in Figure 3 to test your code.</li>

</ol>

You can always do more. Amaze us.

Figure 3: Example circuit

<h2>1.2         Problem 1: Social Network</h2>

You are provided with the following two files: <em>users.csv </em>and <em>edges.csv</em>. The files contain the following:

<ol>

 <li><em>csv </em>has the following attributes:

  <ul>

   <li><strong>user </strong><strong>id</strong>: is a unique identifier of a user</li>

   <li><strong>community</strong>: is one of the following values {science, sport, art}.</li>

   <li><strong>age</strong>: is the age of a user</li>

   <li><strong>posts</strong>: is a list of post types users most frequently share (to simply it for you I set maximum possible per user to 10). It can be one of the following values: {video, image, article}.</li>

  </ul></li>

 <li><em>csv </em>has the following attributes:

  <ul>

   <li><strong>user </strong><strong>id, user id </strong>: represents the edge between two user ids

    <ul>

     <li><strong>What should I do?</strong></li>

    </ul></li>

  </ul></li>

</ol>

To solve this task use and adapt the WeightedGraph implementation from the book (ch10). Represent this data as a graph and perform some interesting analysis of the data. You should demonstrate at least three questions asked about the graph. Some of these will require adding methods and new attributes to WeightedGraph.java file or performing it in the driver code.

<ul>

 <li><strong>What is a CSV file?</strong></li>

</ul>

CSV stands for “comma-separated values”. You can load these files in Excel or Libre Office Calc and view them. However, for this project you will need to load it in Java.

<ul>

 <li><strong>Visualisation</strong></li>

</ul>

If you would like to visualize your graph (or a part of it) I suggest using the following library for representing graphs: http://graphstreamproject.org/download/ Go to the Website and download all the three jars from the 1.3 release (gs-core, gs-algo, gs-ui). Make sure to download them somewhere you can find them. I suggest putting all three jars in a folder on the same level as your <em>src </em>folder, and call it <em>lib</em>. In your IDE make sure you add all three jars to your library list (Congifure Build Path -¿ Add external jars). You have to figure out how to use the library. &#x1f642;

<ul>

 <li><strong>Timely report errors or issues</strong></li>

</ul>

If you find an inconsistency in the data, code or similar, report immediately. It’s also part of the process and could bring you even more glory.

&#x1f642;