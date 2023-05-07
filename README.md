Download Link: https://assignmentchef.com/product/solved-ie523-homework-8-pricing-an-american-option-via-trinomial-trees
<br>
<h1>1           Trinomial Trees and Lattices</h1>

Pretty much everything parallels the Binomial Tree from a conceptual sense. If the stock price at discrete time step <em>k </em>is denoted by <em>S<sub>k</sub></em>. In this case, the process <em>S<sub>k </sub></em>is specified as

with probability <em>p<sub>u</sub>, </em>with probability <em>p<sub>d</sub>, </em>with probability 1 − <em>p<sub>u </sub></em>− <em>p<sub>d</sub>.</em>

Just as with the binomial tree whose leaves can be combined to form the binomial lattice, you can get a <em>trinomial lattice </em>from a trinomial tree. To ensure the martingale property

<em>E</em>{<em>S<sub>k</sub></em><sub>+1 </sub>| <em>S<sub>k</sub></em>} = <em>R </em>× <em>S<sub>k</sub>,</em>

where, as with the Binomial Tree. We need to assign<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a>

Just as with the binomial lattice. you can use (<em>k,i</em>) to denote an arbitrary vertex on the trinomial lattice. The vertex (<em>k,i</em>) is connected to {(<em>k </em>+ 1<em>,i </em>+ 1)<em>,</em>(<em>k </em>+ 1<em>,i</em>)<em>,</em>(<em>k</em>+1<em>,i</em>−1)} with the appropriate probabilities along the appropriate arcs. If <em>V </em>(<em>k,i</em>) is value of the option at (<em>k,i</em>), for the european call option we have the recursion

if (<em>k,i</em>) is a terminal node         otherwise

The option price is <em>V </em>(0<em>,</em>0).

You are going to do a little more than this for this programming assignment.

<h1>2           Part 1: Pricing an American-Option using a Trinomial Model by Recursion</h1>

Using my C++ program american option pricing by binomial model.cpp on Compass as reference, write a C++ program that takes as command-line input the values of <em>T,N,r,σ,S</em><sub>0 </sub>and <em>K</em>, and presents the value of an <em>American-Option </em>using a <em><u>trinomial </u></em>model.

<strong>Input</strong>: The command-line input is the same as what I have for the C++ code that priced the European option in lesson 6 of my notes.

<strong>Output</strong>: A sample output that I expect from your code is shown in figure <strong>??</strong>

Figure 1: Sample output (<strong>Note</strong>: 20 divisions will take some time to run on your computer. Be patient. The next part of this assignment will be able to handle a large number of divisions, as you will see.).

<h1>3           Part 2: Pricing an American-Option using a Trinomial Model by Dynamic Programming</h1>

Using my C++ program american option pricing by dynamic programming.cpp on Compass as reference, write a C++ program that takes as command-line input the values of <em>T,N,r,σ,S</em><sub>0 </sub>and <em>K</em>, and presents the value of an <em>AmericanOption </em>using a <em><u>trinomial </u></em>model.

<strong>Input</strong>: The command-line input is the same as what I have for the C++ code that priced the European option in lesson 6 of my notes.

<strong>Output</strong>: A sample output that I expect from your code is shown in figure <strong>??</strong>

Figure 2: Sample output (<strong>Note</strong>: A large number of Divisions should not be a problem when you use Dynamic Programming.)

<a href="#_ftnref1" name="_ftn1">[1]</a> You can verify this at your leisure.