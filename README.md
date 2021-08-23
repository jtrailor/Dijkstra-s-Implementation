# Dijkstras-Implementation
Program implementation of Dijkstra's algorithm in C.

Problem:
Determine the minimum distance between two cities selected by the user. City nodes and the corresponding edge distance is provided in a text file.

Approach:
Program reads data from the file into two arrays of structs. The two arrays are used to construct an adjacency matrix. This matrix is used by an implementation of Dijkstra'a algorithm to determine the minimum distance between two user selected cities. These operations use arrays of structs that are placed in heap memory and passed via pointer. Multiple helper functions live in high-cohesioned files that are responsible for file reading, data cleaning, user input/output and data structure construction.

Challenges:
This implementation contained multiple challenges. The first challenge was figuring out how to implement Dijkstra's algorithm using an adjacency matrix. Next, I struggled to determine the appropriate data structure to use in this program. I ended up using an array implementation due to the frequent access of data, but I also tested implementations using linked lists. Finally, I faced challenges implementing the malloc'd array. Segmentation faults occured often. These were likely due to storing a complex struct structure within the array itself that were accessed frequently. It was also difficult to ensure that all memory was freed without error as identified by valgrind.

Technologies:
C, Algorithms, FileIO, Data Structures

Results:
A functioning tool that returns the minimum distance between two selected cities. Algorithm works for any files of related structure. Please see attached photos of the tool in operation!
