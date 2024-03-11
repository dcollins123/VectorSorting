# VectorSorting
CS 300 Module Two Assignment Guidelines and Rubric
Overview
The focus of these problems will be working with information extracted from a municipal government data feed containing bids submitted for auction of property. All materials for this assignment can be found in the Supporting Materials section below. The data set is provided in two comma-separated files:

eBid_Monthly_Sales.csv (larger set of 12,023 bids)
eBid_Monthly_Sales_Dec_2016.csv (smaller set of 76 bids)
This assignment is designed to explore sorting algorithms by implementing both a selection sort and quicksort of a vector of bids loaded from a CSV file.

We provide a starter console program that uses a menu to enable testing of the sort logic you will complete. It also allows you to pass in the path to the bids CSV file to be loaded, enabling you to try both files. In this version, the following menu is presented when the program is run:

Menu:

Load Bids
Display All Bids
Selection Sort All Bids
QuickSort All Bids
Exit
Enter choice:

The VectorSorting.cpp program is partially completed. It contains empty methods representing the programming interface used to interact with the linked list. You will need to add logic to the methods to implement the necessary behavior. Here are the methods in VectorSorting.cpp that you must complete:

void selectionSort(vector& bids)

void quickSort(vector& bids, int begin, int end)
int partition(vector& bids, int begin, int end)

Prompt
You will need to perform the following steps to complete this activity:

Setup: Begin by creating a new C++ project with a project type of "Hello World C++ Project".

Name the project “VectorSorting”. Remember to pick the correct compiler in Toolchains and click Finish. This will create a simple VectorSorting.cpp source file under the /src directory.
Download the starter program files and copy them to the project’s /src directory, replacing the existing auto-generated ones. Remember to right-click on the project in the Project Explorer pane on the left and Refresh the project so it adds all the new files to the src folder underneath.
Because this activity uses C++ 11 features, you may need to add the -std=c++11 compiler switch to the miscellaneous settings.
Task 1: Implement the selection sort algorithm:

Code the selection sort logic using “bid.title” as the sort field.
Invoke the selectionSort() method from the main() method including collecting and reporting timing results.
Task 2: Implement the quicksort algorithm:

Code the quicksort logic using “bid.title” as the sort field.
Invoke the quickSort() method from the main() method including collecting and reporting timing results.
Here is sample output from running the completed program:

> ./VectorSorting ~/Downloads/eBid_Monthly_Sales.csv
> VectorSorting.exe Downloads\eBid_Monthly_Sales.csv

Loading bids from CSV and performing a selection sort:

Example Input	Choice: 1	Choice: 3 
Display	Menu:
1. Load Bids
2. Display All Bids
3. Selection Sort All Bids
4. QuickSort All Bids
9. Exit
Enter choice: 1	Menu:
1. Load Bids
2. Display All Bids
3. Selection Sort All Bids
4. QuickSort All Bids
9. Exit
Enter choice: 3
Output	Loading CSV file
eBid_Monthly_Sales.csv
12023 bids read
time: 12023 clock ticks
time: 0.173945 seconds	12023 bids sorted
time: 10623604 clock ticks
time: 10.6236 seconds
Loading bids from CSV and performing a quicksort:


Example Input	Choice: 1	Choice: 4 
Display	Menu:
1. Load Bids
2. Display All Bids
3. Selection Sort All Bids
4. QuickSort All Bids
9. Exit
Enter choice: 1	Menu:
1. Load Bids
2. Display All Bids
3. Selection Sort All Bids
4. QuickSort All Bids
9. Exit
Enter choice: 4
Output	Loading CSV file
eBid_Monthly_Sales.csv
12023 bids read
time: 174985 clock ticks
time: 0.174985 seconds	12023 bids sorted
time: 47964 clock ticks
time: 0.047964 seconds
Note the dramatic difference in the time it takes to sort over 12,000 records - 10.6 seconds versus 4 hundredths of a second!

Your assignment submission must address the following rubric criteria:

Code Reflection: A brief explanation of the code and its purpose, and a brief discussion of your experience in developing it, including any issues that you encountered while completing the exercise and what approaches you took to solve them
Pseudocode or Flowchart: A pseudocode or flowchart description of the code that is clear and understandable and captures accurate logic to translate to the programming language
Specifications and Correctness: Source code must meet its specifications and behave as desired. Correct code produces the correct output as defined by the data and problem; however, you should also produce fully functioning code (with no errors) that aligns with as many of the specifications as possible. You should write your code in such a way that the submitted file executes, even if it does not produce the correct output. You will be given credit for partially correct output that can be viewed and seen to be partially correct.
Annotation / Documentation: All code should also be well-commented. This is a practiced art that requires striking a balance between commenting everything, which adds a great deal of unneeded noise to the code, and commenting nothing. Well-annotated code requires you to:
Explain the purpose of lines or sections of your code, detailing the approach and method you took to achieve a specific task in the code.
Document any section of code that is producing errors or incorrect results.
Modular and Reusable: Programmers should develop code that is modular and reusable. If it contains functionality and responsibility in distinct methods, code is more flexible and maintainable. Your code should adhere to the single responsibility principle—classes and methods should do only one job. If you can replace a method with another that uses a different technique or implementation without impacting (having to refactor or rewrite) other parts of your code, then you have succeeded in creating modular methods.
Readability: Code needs to be readable to a knowledgeable programmer. In this course, readable code requires:
Consistent, appropriate whitespace (blank lines, spaces) and indentation to separate distinct parts of the code and operations
Explicit, consistent variable names, which should clearly indicate the data they hold and be formatted consistently: for example, numOrders (camelCase) or item_cost (underscored)
Organized structure and clear design that separates components with different responsibilities or grouping-related code into blocks
What to Submit
To complete this assignment, submit the CPP code files and a code reflection and associated pseudocode or flowchart written portion. Your written portion should be 1–2 paragraphs in length.

Supporting Materials
CS 300 Vector Sorting Assignment Student Files.zip
Download this zipped file folder to begin your assignment. The data sets you will use in this assignment are provided in these comma-separated files:

eBid_Monthly_Sales.csv (larger set of 12,023 bids)
eBid_Monthly_Sales_Dec_2016.csv (smaller set of 77 bids)
VectorSorting.cpp program, which is a partially completed program that you can use as a starting point for the assignment
