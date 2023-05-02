Download Link: https://assignmentchef.com/product/solved-comp2710-homework-6-a-class-named-doctor
<br>
Create a class named Doctor that has three member variables:

<ul>

 <li>name – A string that stores the name of the doctor</li>

 <li>numPatients – An integer that tracks how many patients the doctor must treat</li>

 <li>patientList – A dynamic array of strings used to store the patient names</li>

</ul>

Write appropriate constructor(s), mutator, and accessor methods for the class along   with the following:

<ul>

 <li>A method that inputs all values from the user, including the list of patient names. Note that this method has to support input for an arbitrary number of patient.</li>

 <li>A method that outputs the name and list of all patients.</li>

 <li>A method that resets the number of patient to 0 and the patientList to an empty list.</li>

 <li>An overloaded assignment operator that correctly makes a new copy of the list of patients.</li>

 <li>A destructor that releases all memory that has been allocated.</li>

</ul>

Write a main function that tests (i.e., unit testing) all of your functions.

<strong><em><u>Requirements:</u> </em></strong>

<ol>

 <li>(5 points) Use comments to provide a heading at the top of your code containing your name, Auburn Userid, filename, and how to compile your code. Also describe any help or sources that you used (as per the syllabus).</li>

 <li>(5 points) Your source code file should be named as “hw6.cpp”.</li>

 <li>(5 points) Your program must use dynamic array</li>

 <li>(5 points) Your program must use strings</li>

 <li>(5 points) A method that inputs all values from the user</li>

 <li>(5 points) A method that outputs the name and list of all patients.</li>

 <li>(5 points) A method that resets the number of patient to 0 and the patientList to an empty list.</li>

 <li>(10 points) An overloaded assignment operator</li>

 <li>(5 points) A destructor</li>

 <li>(15 points) Correctly implement the main function (i.e., unit testing).</li>

 <li>(10 points) Creating two versions using conditional compilation.</li>

 <li>(5 points) You must limit the number of global variables and data 13. (15 points) Usability of your program (e.g., user interface)</li>

 <li>(5 points) Readability of your source code.</li>

</ol>

Note: You will lose <strong>at least 20 points (and up to 40 points)</strong> if there are compilation errors or warning messages when the TA compiles your source code. You will lose points if you: do not use the specific program file name, or do not have a comment on each function in your program you hand in.




<strong><em><u>How to Create Two Versions?</u> </em></strong>

You can use the preprocessor directive #ifdef to create and maintain two versions (i.e., a debugging version and a

product version) in your program. If you have the sequence

#ifdef UNIT_TESTING

add your unit testing code here

#else

add your code for the product version here

#endif

in your program, the code that is compiled depends on whether a preprocessor macro by that name is defined or not. For example, if there has been a “#define UNIT_TESTING” macro line), then “ add your unit testing code here ” is compiled and “ add your code for the product version here ” is ignored. If the macro is not defined, “ add your code for the product version here ” is compiled and “ add your unit testing code here ” is ignored.

These macros look a lot like if statements, but macros behave completely differently. More specifically, an if statement decides which statements of your program must be executed at run time; #ifdef controls which lines of code in your program are actually compiled.

<strong><em><u>Unit Testing:</u> </em></strong>

Unit testing is a way of determining if an individual function or class works. You need to isolate a single function or class and test only that function or class. For each function in this homework, you need to check <u>normal cases and boundary</u> <u>cases.</u>

Examples for tested values:

<ul>

 <li>string – empty string, medium length, very long</li>

 <li>Array – empty array, first element, last element Int – zero, mid-value, high-value</li>

</ul>

You must implement a unit test driver for each function implemented in your program. You may need to use assert() to develop your unit test drivers if tested results are predictable.2


