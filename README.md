java c
Module code and Title 
DTS103TC Design and Analysis of Algorithms School Title 
School of AI and Advanced Computing Assignment Title 
Coursework Submission Deadline 
Sunday, March 23rd 23:59 (UTC+8 Beijing), 2025 
DTS103TC Design and Analysis of Algorithms 
Individual Coursework
Due: Sunday   March   23rd, 2025 @   11:59pm
Weight: 40%
Maximum score: 100 points
Learning Outcomes Assessed 
•   A.   Describe   the   different   classes   of algorithms   and   design   principles   associated   with   them;   Illustrate   these   classes   by   examples   from   classical   algorithmic   areas,   current   research   and   applications.
•   B.   Identify   the   design   principles   used   in   a   given   algorithm,   and   apply   design   principles   to   produce efficient algorithmic solutions to a given problem.
•      C.   Have   fluency   in   using   basic   data   structures   in   conjunction   with   classical   algorithmic   problems.
General notes 
•   Please   read   the   coursework   instructions   and   requirements   carefully. Not   following   these   instructions   and requirements may result in loss of   marks.
•   The assignment must be submitted via Learning Mall to the correct drop box.   Only electronic   submission is accepted and   no hard copy   submission.
•   All   students must download their file and check that   it   is   viewable   after   submission.Documents   may   become   corrupted   during   the   uploading   process   (e.g.         due   to   slow   internet   connections).    However,   students   themselves   are   responsible   for   submitting   a   functional   and   correct file for assessments.
•   Academic Integrity Policy is strictly followed.
•   The use of   Generative AI for content generation is not permitted on   this assessed coursework.   Submissions will be checked through Turnitin.
Coding Policy 
• Programming Language: All code   must   be   written   in Python, with a   version of   3.6 or   higher.   Students   are required to use Jupyter Notebook for   their   implementation,   and   the   main   file   must be an ’   .ipynb’ file that includes all outputs (such as printed results, graphs, etc).
• Code Structure: The   code   must   be   well-structured,   readable, and   properly   documented.   Comments   should   be   included   for each   function and section, explaining   its   purpose and   functionality.   Each notebook cell must contain   at one   task   only.    In   other   words,   you   can   use   several   cells   for   one   task but one cell cannot contain more than one   task. 
• Libraries and Tools: Do not use any libraries or tools.   Only the Python builtins and classes   provided during the labs are allowed.   For example, the class Node is   allowed.
• Code Validation: Ensure   the code   is   fully executable   without errors   for each   Jupiter   Notebookcell. All notebooks must be submitted with outputs included (e.g., printed results, graphs, etc),   allowing the marker to verify the results without rerunning the notebook.   Of   course, the code   of   the cell must match the output of   the cell.
Submission Policy 
1. Submission Format 
•   Each student must submit a single ZIP file containing:
(a)   The final report in PDF format.    The first page   of   the   PDF   report   must   be   the   cover   sheet provided on Learning Mall.
(b)   A single Jupyter Notebook (file name ending with   .ipynb) must be provided.
2. File Naming 
• The   ZIP   file   must   be   named   in   the   format: Lastname_Firstname_StudentID_Coursework.zip.
• The   PDF   report   must   be   named   in   the   format: Lastname_Firstname_StudentID_Coursework.pdf.
•   Each   individual’s   code   must   be   named   in   the   format:   Lastname_Firstname_StudentID_Code   .ipynb.
Late Policy 
5% of   the total marks available for the assessment shall be   deducted from the   assessment   mark   for   each working day after the submission date, up to a maximum of   five working days.
Avoid Plagiarism 
•   Do not submit work from other students.
•   Do not share code/work to other   students.
•   Do not read code/work from other students, discussions should be   limited to high level only.
•   Do not use open-source code.   You must write your own solution and comment your   code.
Overview In   this   coursework,   you   are   expected   to   design   and   implement   algorithms   to   produce   solutions   to   four   given   problems   in   Python.    You   should   have   function(s)   to   receive   task   input   as   parameters,   implement your algorithm design and return results.
1 Task 1 (20 marks) Given an m ×   n grid filled with integers representing the weight of   the crop in one cell (or crop area).   A farmer (who is gathering the crops) starts at the top left cell and need to find a way to the bottom   right cell.   The farmer can only move either down or right. What is the maximum weight of   cro代 写DTS103TC Design and Analysis of AlgorithmsPython
代做程序编程语言ps the   farmer can collect through its path from top left to   bottom   right?    Solve this problem with   dynamic   programming.
Example   1 of   input grid:
10         4            8            3
6            7            5            1
2         4            2            2
Output:   32 because   the   path   giving   the   maximum   reward   is   10,   6,   7,   5,   2,   2.
Example 2 of   input grid:
10         4            8            3
6            7            5            1
20         4            2            2
Output:   44 because   the   path   giving   the   maximum   reward   is   10,   6,   20,   4,   2,   2.
You should have a function named maxPathSum to   receive   the   grid   (List[List[int]])   and   return   the   maximum reward (int).
2 Task 2 (20 marks) 
Given a directed acyclic graph, use depth first search to find all the   paths from   node   S   to   node T.   Input example:
graph      =      {"S":      ["A","B"],
"A":    ["B","T"],
"B":      ["T"]}
Output:
[["S",      "A",      "T"],
["S",      "A",      "B",      "T"],   ["S",      "B",      "T"]]
Answer:   There   are   three   paths:   S   →   A → T,   S   →   A   →   B   →   T,   S   →   B   →   TThe adjacency list of   the graph can be represented using a dictionary in python, where the keys are   the nodes of   the graph, and their values are   a list   storing the   neighbors   of   these   nodes.   You   should   have a function named allPaths to receive the adjacency list represented as a dictionary and return   a list of   paths.
3.1 Introduction A factory is producing n = 2l   objects such that they all have the same weight w.   However, the objects   sometimes   have   a   different   weight   and   must be   identified.    Suppose   we   are   in   the   case   where   two   objects   among the n have different weights   such   that   the   first   object   has   weight   w1    and   the   second   object has weight w2    with the following properties:    w1      < w2 < w and w1 + w2 = w. Given a list of weights, implement an efficient algorithm to find the index of the two objects with weight different than w. In this problem, we use a precision digital balance to measure accurately the total weight of a list of objects.
Input/Output pair example:   weights      =    [w,    w,    w,   w_2,   w,   w,   w_1,   w],    (3,    6)
In this example, there are n   =   23      =   8   weights   where   w1    is at   index   6   and   w2    is   at index   3.    In other   words,   (i1,   i2) =   (3,   6) and, in   Python, we   have   weights[6]    =    w_1 and   weights[3]    =    w_2.
The   Python   function   containing   your   algorithm   must   be   named   findWeights2   with   function   argument   named   weights   to   receive   a   list   of   float   numbers. The   output   of   your   function   is   a   tuple   of   index (i1,   i2).
3.2       Algorithm design 
This section is meant to guide the   student through   solving   the   problem.    Suppose we   divide the   set   of   input objects in two disjoint subsets U1    and U2    of   equal sizes.
1.   At the first iteration (first division of   the object list):   how many objects are there in U1    and U2? 
2.   What   are   the   possible   values   for   the   weight   difference   between   U1    and   U2?    (Hint:    negative   weight differences are considered)
3.      In   each   case, in   which   set   does   w1   belong   to?   What   about   w2?
4.      In each case, what should the algorithm do?   (4   points)
5.   A sub-problem:   we consider a simpler version of   the problem with the following conditions:
•   There   are   n   =   2l      objects.
•   Among the n objects, only one object has weight w0    < w.The   Python   function   containing   your   algorithm   must   be   named   findWeight1   with   function   argument   named   weights   to   receive   a   list   of float   numbers.    The   output   of your   function   is   an index i.
6.   Based   on   the   previous   questions,   implement   an   efficient   algorithm   (the   function   is   named   findWeights2) to find the positions ofw1    and w2   . You may reuse the findWeight1 function.
7.   What is the running time of   your algorithm?
4       Task 4 (30 marks)
Given a list of   intervals, merge all overlapping intervals and return the merged list.
Input example:      [[9,11],    [1,4],    [13,19],      [2,7]]
Output: the merged list should be   [[1,7],    [9,11],      [13,19]].
1.      Identify the appropriate data structures and algorithms needed to solve this problem.   For each   choice, explain your solution in less than 200 words.
2.      Implement your solution in Python language.   The function   should be   named mergeIntervals   and receive as input   as Python List
3.   Provide 5 test cases of   your algorithm.
4.   Analyze the time and space complexity of   your algorithm.





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
