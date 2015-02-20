##Tyler Cox, 11:45
--------------------------------------------------------------
###Suture Packaging

Description: Write a program that reads a data file containing data on batches of rejected sutures, and then analyzes and reports on this data.  Write the output to a file.  This output file will have your name or names, and the results in terms of percent of failures in each category, the total numbers in each category and the total number of batches rejected. Also, you need to check that all data is correct, that it is actually a rejected batch.  

Input: data file
Output: output file with names, percent failure of category, total number in each category, number of rejected batches

Functions:

Program:

1. initialize fin, fout    //for importing and exporting data
2. do-while loop to read the data   //means we dont have to enter into it before

    - condition: !fin.eof()
    - //do stuff to test if it's a good file
    - //do other stuff here to analyze
    
--------------------------------------------------------------
###Heron's Formula

Description: Write, test and execute a function that has inputs a, b, c.  The function should compute s first.  If the value of s is positive, then the function computes and returns the area A.  If s is negative, then a, b, and c do not form a triangle, and the function should return A = -1 and let the user know that there is an error.  You do not need input or output files for this problem.  

Input: side_a, side_b, side_c
Output: area

Functions: A = sqrt([s(s-a)(s-b)(s-c)]), s = ((a+b+c))/2

s_calc(double a, double b, double c)
    { return ((a+b+c))/2 }

Program:

1. initialize variables: double a, b, c, s, A
2. user input for side lengths -> a, b, c
3. use s_calc(a, b, c) to compute s
    - if s is negative: print an error occurred, A = -1
    - if s is positive: 
        A = sqrt([s(s-a)(s-b)(s-c)])
        print A
