Download Link: https://assignmentchef.com/product/solved-cpsc-331hw2-codes
<br>
This assignment consists of two parts. The first part consists of problems that will give you more practice working with linear structures, recursion and recurrence relationships. The second part consists of short coding exercises that will give you additional practice with Java generics, linked lists and recursion.

<h1>Part I</h1>

<ol>

 <li>(5 points)</li>

</ol>

Provide pseudocode for a recursive version of selection sort that operates on an array of <em>n </em>elements. Use your pseudocode to set up a recurrence relation for the total number of comparisons performed. Solve the recurrence relation to determine the asymptotic complexity of selection sort.

<ol start="2">

 <li>(5 points)</li>

</ol>

The Catalan numbers are defined recursively as:

<em>.</em>

Use this definition to determine <em>C</em><sub>3</sub>. Illustrate your answer using a recursion call tree assuming a na¨ıve recursive implementation.

<ol start="3">

 <li>(5 points)</li>

</ol>

Determine an asymptotic upper bound for the following recurrence relations. Assume that the cost of the base case is a constant.

<ul>

 <li><em>T</em>(<em>n</em>) = 2<em>T</em>(<em>n </em>− 1) + 1</li>

 <li><em>T</em>(<em>n</em>) = <em>T</em>(<em>n </em>− 1) + <em>T</em>(<em>n/</em>2) + <em>n</em></li>

</ul>

<h1>Part II</h1>

<ol>

 <li>(10 points)</li>

</ol>

In this exercise, you are asked to write code to sort a <em>singly linked list </em>using bubble sort. You will also get additional practice with generic classes and methods.

We went over bubble sort in class. In the class version of bubble sort, we go over the array from right (higher indices) to left (lower indices) in each pass and swap adjacent elements that are out of order. During each pass the smallest element bubbles to the left to its appropriate spot. Think about the changes that are needed if, in each pass, we scan the array from left to right and the largest element bubbles to the right to its appropriate spot. Now think about what we would need to do if, instead of an array, we were using a singly linked list, and in each pass, we scanned the list from left to right and swapped adjacent elements that are out of order.

Two files are provided for this exercise:

<h2></h2>

SLLNode.java – Represents a node in a singly linked list.

SLL.java – A class that encapsulates a singly linked list. Helper methods are provided to add and remove elements, and to query the size.

Implement a generic static method called BubbleSort that takes a singly linked list as an input and sorts it <em>in place </em>using bubble sort. Your method should have the following signature:

public static &lt;T extends Comparable&lt;? super T&gt;&gt; void BubbleSort( SLL&lt;T&gt; list )

Please encapsulate your method in a class called SLLBubbleSort.

Your implementation should only rely on the classes SLLNode.java and SLL.java. You are not allowed to use any classes from the Java collections framework. Test your program with lists consisting of different types of Comparable elements (Integers, Doubles, Strings etc.).

<ol start="2">

 <li>(5 points)</li>

</ol>

A prefix expression is one where the operator appears before the operands. Like the postfix notation, it is also parentheses-free. The order of evaluation is determined by the order in which the operators and the operands appear. For example:

+ * 3 2 6 = + 6 6 = 12

+ – 2 * 3 4 5 = + – 2 12 5 = + -10 5 = -5

Write a recursive method in Java that evaluates a prefix expression. Your method should be encapsulated in a file called Prefix.java that has the following class structure:

public class Prefix {

public static int evaluate( Scanner sc ) {

// your recursive evaluation code

}

}

Please note that you are required to use recursion for the evaluation. You can assume that the provided expression will be in valid prefix notation.


