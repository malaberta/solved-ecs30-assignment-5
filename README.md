Download Link: https://assignmentchef.com/product/solved-ecs30-assignment-5
<br>
In this assignment, you will download Program5Source.zip and complete the code fragments as described below.

Problem 1: deletespaces.c

I this problem you will write a program that reads a string, deletes any whitespace from the string, and prints the result back to the user. Read the string using fgets, a safe way to read in strings. To read a string of length at most n into char* str, use the following: fgets(str, n + 1, stdin);

Generally, fgets is used to read a string from a file, but using stdin as the third argument causes fgets to read a string from stdin instead. Example output:

[<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="334140544a40565f7343500204">[email protected]</a> ~]$ ./deletespaces

Enter a max string length: 99

Enter the string to delete whitespace from: The Quick Brown Fox Jumps Over The Lazy Dog Result:

TheQuickBrownFoxJumpsOverTheLazyDog

[<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="1d6f6e7a646e78715d6d7e2c2a">[email protected]</a> ~]$ ./deletespaces

Enter a max string length: 20

Enter the string to delete whitespace from: a bcd ef g hi

Result: abcdefghi

1

Problem 2: matrixaddition.c (50 points, 5 per test case)

In this problem you will implement integer matrix addition. This will require you to dynamically allocate space for a 2 dimensional array. An example of matrix addition is:

In general, if <em>A </em>and <em>B </em>are matrices with the same number of rows and columns, then their sum <em>C </em>= <em>A </em>+ <em>B </em>is defined by <em>C</em>[<em>i</em>][<em>j</em>] = <em>A</em>[<em>i</em>][<em>j</em>] + <em>B</em>[<em>i</em>][<em>j</em>]. Here, <em>A</em>[<em>i</em>][<em>j</em>] is the integer in the <em>i</em><sup>th </sup>row and <em>j</em><sup>th </sup>column of <em>A</em>. In the example above, <em>A</em>[1][1] = 1, <em>A</em>[1][3] = 3, and <em>A</em>[2][2] = 8.

This program has been partially written for you in matrixaddition.c. Write the body of functions that are marked with a comment that begins with

// Homework TODO: …

Do not modify other parts of the code. Example output:

[<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="215352465852444d6151421016">[email protected]</a> ~]$ ./matrixaddition Enter the number of rows and columns: 2 2 Enter matrix A:

Input row 0 elements, separated by spaces: 1 0

Input row 1 elements, separated by spaces: 0 1 Enter matrix B:

Input row 0 elements, separated by spaces: 2 2

Input row 1 elements, separated by spaces: 3 4

A + B =

3 2

3 5

[<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="5e2c2d39272d3b321e2e3d6f69">[email protected]</a> ~]$ ./matrixaddition Enter the number of rows and columns: 3 6 Enter matrix A:

Input row 0 elements, separated by spaces: 1 2 3 4 5 6

Input row 1 elements, separated by spaces: 0 0 0 0 0 0 Input row 2 elements, separated by spaces: 10 5 23 84 91 2

Enter matrix B:

Input row 0 elements, separated by spaces: 9 8 7 6 5 4

Input row 1 elements, separated by spaces: 2 1 2 1 2 1

Input row 2 elements, separated by spaces: 14 83 62 93 45 32

A + B =

10 10 10 10 10 10

2 1 2 1 2 1

24 88 85 177 136 34

2