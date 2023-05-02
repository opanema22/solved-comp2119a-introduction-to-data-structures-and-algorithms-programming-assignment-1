Download Link: https://assignmentchef.com/product/solved-comp2119a-introduction-to-data-structures-and-algorithms-programming-assignment-1
<br>
<ul>

 <li><strong>[O4]. Implementation</strong></li>

</ul>

<strong>[O4] </strong>In this assignment, you are requested write a program to solve four tasks, <strong>A</strong>, <strong>B</strong>, <strong>C </strong>and <strong>D</strong>, using ADT we learned during class.

Your program will be judged by a computer automatically, please follow the exact format. You should read from standard input and write to standard output. e.g, scanf/print, cin/cout.

<strong>Languages.</strong>

We only accept C/C++ programming languages.

<strong>Judging.</strong>

Please note that your solution is automatically judged by a computer.

Solutions that fail to compile or execute get 0 points.

We have designed 40 test cases, 10 for each task. Each test case is of 2.5 points.

The time limit for each test case is 1 second.

For each test case, you will get 2.5 points if your program passes it otherwise you will get

0.

<strong>Self Testing.</strong>

You should test your program by yourself using the provided sample input/output file.

The sample input/output is <strong>different </strong>from the ones used to judge your program, and it is designed for you to test your program by your own.

Note that your program should always use standard input/output.

To test your program in Windows:

<ol>

 <li>Compile your program, and get the executable file, “main.exe”</li>

 <li>Put sample input file, “input.txt”, in the same directory as “main.exe”</li>

 <li>Open command line and go to the directory that contains “main.exe” and “input.txt”</li>

 <li>Run “main.exe <em>&lt; </em>txt <em>&gt; </em>myoutput.txt”</li>

 <li>Compare myoutput.txt with sample output file. You may find “fc.exe” tool useful.</li>

 <li>Your output needs to be <strong>exactly </strong>the same as the sample output file.</li>

</ol>

To test your program in Linux or Mac OS X:

<ol>

 <li>Put your source code “main.cpp” and sample input file “input.txt” in the same directory.</li>

 <li>Open a terminal and go to that directory.</li>

 <li>Compile your program by “g++ main.cpp -o main”</li>

 <li>Run your program using the given input file, “./main <em>&lt; </em>txt <em>&gt; </em>myoutput.txt”</li>

 <li>Compare myoutput.txt with sample output file.</li>

 <li>Your output needs to be <strong>exactly </strong>the same as the sample output file.</li>

 <li>You may find the <strong>diff </strong>command useful to help you compare two files. Like “diff -w myOutput.txt sampleOutput.txt”. The −<em>w </em>option ignores all blanks ( SPACE and TAB characters)</li>

</ol>

Note that myoutput.txt file should be <strong>exactly </strong>the same as sample output. Otherwise it will be judged as wrong.

<strong>Submission.</strong>

Please submit your source files through moodle.

You should submit four source files(<strong>without </strong>compression), one for each task.

Please name your files in format UniversityNumber-X.cpp for <em>X </em>in {A, B, C, D}, e.g. 1234554321-A.cpp.

<strong>Task A</strong>

Given an empty stack and some operations (<em>push </em>and <em>pop</em>) on the stack, print the popped element for each <em>pop </em>operation. When applying <em>pop </em>operation on an empty stack, output ‘false’ and then terminate the program. The number of operations is at most 1000. The elements of the stack are integers. All inputs in the test case are valid. (You don’t need to consider the case when format of input is wrong.)

You should implement a stack by yourself without using built-in classes.

<strong>Input:</strong>

The input contains multiple lines, where each line contains one operation.

<strong>Output:</strong>

Print the results, seperated by spaces. Having a trailing space at the end of the line or not does not matter.

<strong>Examples:</strong>

<ol>

 <li>Input:</li>

</ol>

push 1 push 2 pop push 9 pop

Output:

2 9

<ol start="2">

 <li>Input:</li>

</ol>

push 3 push 12 pop pop pop push 4 pop

Output:

12 3 false

<strong>Task B</strong>

Rearrange a singly linked list in such a way that all odd nodes together followed by the even nodes. Note that here we are talking about the node number and not the value in the nodes. Your program should run in <em>O</em>(1) space complexity and <em>O</em>(<em>n</em>) time complexity. The first node is considered odd, the second node even and so on. 1 ≤<em>n</em>≤ 1000.

Note: You must refer to the folder ‘sketch for B’: do not change the code in main.cpp and ListNode.h, and you are only allowed to edit 1234554321-B.cpp. You just need to submit

1234554321-B.cpp at the end. (Use your own university number.)

<strong>Input:</strong>

The input contains two lines.

The first line contains an integer <em>n </em>– length of the list.

The second line contains <em>n </em>distinct integers, standing for the list.

<strong>Output:</strong>

Print the required list, containing <em>n </em>integers. Having a trailing space at the end of the line or not does not matter.

<strong>Examples:</strong>

<ol>

 <li>Input:</li>

</ol>

6

<ul>

 <li>5 3 7 8 11</li>

</ul>

Output:

1 3 8 5 7 11

<ol start="2">

 <li>Input:</li>

</ol>

7

<ul>

 <li>1 3 5 6 4 7</li>

</ul>

Output:

2 3 6 7 1 5 4

<strong>Task C</strong>

Given a parentheses string <em>s</em>, compute the score of the string based on the following rule:

<ul>

 <li>If <em>s </em>is not balanced, the score is 0.</li>

 <li>() has score 1.</li>

 <li>AB has score A + B, where A and B are balanced parentheses strings.</li>

 <li>(A) has score 2 * A, where A is a balanced parentheses string.</li>

</ul>

A balanced string satisfies the following requirements:

<ul>

 <li>The number of ‘(’ equals the number of ‘)’ in the string.</li>

 <li>Counting from the first position to any position in the string, the number of ‘(’ is greater than or equal to the number of ‘)’ in the string. (For example, ‘)(’ is not balanced.)</li>

</ul>

The length of <em>s </em>is at most 30.

<strong>Input:</strong>

The input is a parentheses string <em>s</em>.

<strong>Output:</strong>

Print the score of <em>s</em>.

<strong>Examples:</strong>

<ol>

 <li>Input:</li>

</ol>

(())

Output:

2

<ol start="2">

 <li>Input:</li>

</ol>

(()(()))

Output:

6

<ol start="3">

 <li>Input:</li>

</ol>

((()())

Output:

0

<strong>Task D</strong>

Given <em>n </em>strings, output the number of distinct strings. The sum of length of strings is at most 10<sup>6</sup>.

<strong>Input:</strong>

The input contains two lines:

The first line is an integer <em>n</em>, which is the number of strings in the second line. The second line are <em>n </em>strings.

<strong>Output.</strong>

Output an integer – the number of distinct strings.

<strong>Examples.</strong>

<ol>

 <li>Input: 3 abc abcc abd Output:</li>

</ol>

3

<ol start="2">

 <li>Input: 7</li>

</ol>

aaa bbb abc bjyx wegdbs szdszd aaa Output:

6

<ol start="3">

 <li>Input: 5</li>

</ol>

abc lgieong lgieong kkkk lgieong Output:

3