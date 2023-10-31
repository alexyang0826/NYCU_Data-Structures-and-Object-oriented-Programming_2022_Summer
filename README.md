# NYCU_Data-Structures-and-Object-oriented-Programming_2022_Summer
 
## Programming Assignment One

**Requirement Specification**: All the calculations should be done in double precision. Define a variable as double type for floating point computation. Don’t use float. Show the value of a floating point number up to 8 decimal digits.
A.	Basic tasks.
I.	Write your name in the header file mySystemApp.h
II.	Press ‘s’ or ‘S’ to show your student information:  date, student ID, name, and email address. showMyStudentInfo_2021_Summer( ) in mySystemApp.cpp
III.	Set STUDENT_INFO for your name and student ID in mySystemApp.cpp.
Items I, II and III must be done. If not, your score is zero.	
Key usages:
F1: perform Monte Carlo Simulation
F3: perform Quatic Function Calculation
F4: perform the student record management
i, I: ask for input
s, S: show the student information 
In mySystem_MonteCarlo, implement the followings.
1.	Show a message about the Monte Carlo simulation.
2.	Press ‘i’ or ‘I’ to ask the user to input the radius of a circle. The radius is inside [1,10]. Ask the user to input the number of samples. The number of samples is between 1 and 1,000,000.
3.	Press ‘1’ to set the option to MCS_OPTION_CIRCLE. Use mOption.
4.	Press ‘2’ to set the option to MCS_OPTION_FUNC_01. Use mOption.
5.	Use the Monte Carlo simulation to estimate the area of the region. Show the estimated area value. Use generateUniformSample ( ) to generate samples. Use computeValue( ) to compute the area of the region. Use mValue to store the area.
6.	Implement getValue( )
7.	Get the radius getRadius( ).
8.	Get the number of samples getNumSamples( ).
9.	Implement isInsideRegion( ) 
10.	Implement getSample( … ).
11.	Implement reset( ) to recompute the samples and the area of the region.
12.	Get the coordinates of a sample based on the sample index (starting from 0). Return true if the sample lies inside the region. Otherwise return false. 
13.	Press ‘<’ to decrease the number of sampler points by 5000 each time. Compute the new samples. Implement method decrease( ). The minimum number of sample points is 2.
14.	Press ‘>’ to increase the number of sampler points by 5000 each time. Compute the new samples. Implement method increase( ). The maximum number of sample points is 1,000,000.
15.	Press ‘n’ to decrease the radius of the circle by 1. The smallest radius is 1. Compute the new samples and output the area of the region. Implement method decreaseRadius( ).
16.	Press ‘m’ to increase the radius of the circle by 1. The largest radius is 10. Compute the new samples and output the area of the region. Implement method increaseRadius( ).

The center of the circle is at the origin, i.e., (0,0).
The region is defined as follows:
When Option = MCS_OPTION_CIRCLE, the region is inside the circle.
When Option = MCS_OPTION_FUNC_01, the region is inside the circle and also a point (x,y) is inside the region iff the condition y >= sin(x) + cos(x) is true.


 
In mySystem_QuarticFunction, implement the following items.
1.	Press ‘i’ to ask the user to input the range of x, i.e., minimum value and maximum value of x. The minimum and maximum values should be in the interval [-100, 100]. Ask the user to input the number of sample points inside the interval [2, 500].
2.	Get the range of x, i.e., getRangeOfX.
3.	Get the number of sample points, i.e., getNumOfSamples.
4.	Get the value of the function for a given x value, i.e., getValue.
5.	Press ‘1’, set a = 1.0*k, b = -1.0*k, c = 2*k, d = 15*k,  e = 100.0*k.
6.	Press ‘2’, set a = -1.0*k, b = -5.0*k, c = 2*k,  d = 15*k, e = 0*k;.
7.	Press ‘3’, set a = 1.0*k, b = 1.0*k, c = -20*k, d = 15*k,  e = 300.0*k.
8.	Press ‘4’, set a = 1.0*k, b = 5.0*k, c = 20*k, d = -35*k, e = -100*k;
9.	Press ‘v’ to decrease value b by 0.0002.
10.	Press ‘b’ to increase value b by 0.0002.
11.	Press ‘n’ to decrease value c by 0.002.
12.	Press ‘m’ to increase value c by 0.002.
13.	Press ‘,’ to decrease value d by 0.02.
14.	Press ‘.’ to increase value d by 0.02.

k = 0.002.
The quartic function is: f(x) = ax4 + bx3 + cx2 + dx + e
Set the initial values to a, b, c, d, and e, e.g., c = d = 0.5; a = 1.0; b = -0.5; e = 0.0;
Play with the system by changing the coefficient values, i.e., b, c, and d. See how the curve of the function change accordingly. Do you observe some interesting patterns?

In mySystem_StudentManager, implement the following items.
1.	Press ‘i’ or ‘I’ to ask for input.
2.	Ask the user to input the number of students. The number of students is in [2,100].
3.	Ask the user to input the score of each student. The score range is [0, 100]. The score value is an integer.
4.	Show the range of the scores.
5.	Show the average score.
6.	Show the standard deviation of the scores.
Standard deviation = sqrt( sum(x – x’)*( x – x’)/(n-1) ), for scores of all students, where x is the score of a student and x’ is the average. Read the article about standard deviation in Wiki if you are not sure what it is. 
7.	Show the scores in an ascending order. That is, sort the scores.
8.	Get the number of students whose score is inside an interval [s0, s1] (inclusive). Implement getNumOfStudentsInScoreInterval(…).
The program shows the histogram of the scores of all the students.


Use ( rand( ))/(double) (RAND_MAX)
to compute  a random value between [0, 1].

## Programming Assignment Two
**Requirement Specification**

A.	Basic tasks.
I.	Write your name, student ID and email address in the header file mySystemApp.h
II.	Press ‘s’ or ‘S’ to show your student information:  date, student ID, name and email address. showStudentInfo_2021_Summer( ) in mySystemApp.cpp
III.	Set your name and ID for cn_StudentInfo in mySystemApp_HandleEvents.cpp
IV.	Press F5 to show student information at the top bar of the window.
Items I, II, III and IV must be done. If not, your score is zero.	
Key usages:
F1: perform Graph System
F4: perform Image System
F5: show your student information. Change cn_StudentInfo if necessary. 
i, I: ask for input (to see other key usages in the current system)
s, S: show the student information 

B.	System tasks.
[50%] Implement GRAPH_SYSTEM. You can see the details in the header and source files (mySystem_GraphSystem).

[50%] Implement the image system. You can see the details in the header and source files (mySystem_ImageEditor.h, mySystem_ImageEditor.cpp, mySystem_ImageEditor_draw.cpp).
