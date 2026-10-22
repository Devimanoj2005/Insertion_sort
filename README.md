Insertion Sort Algorithm

1. Objective

To implement the Insertion Sort algorithm using the C programming language and analyze its time and space complexities using asymptotic notations.

2. Programming Language

C

3. Algorithm

1. Start.
2. Read the number of elements "n".
3. Read the array elements.
4. Start from the second element of the array.
5. Store the current element in "key".
6. Compare "key" with the previous elements.
7. Shift all elements greater than "key" one position to the right.
8. Insert "key" into its correct position.
9. Repeat steps 4–8 until all elements are processed.
10. Display the sorted array in ascending order.
11. Stop.

4. How to Run

Prerequisites

- Install a C compiler, such as GCC.
- Save the source code as "insertion_sort.c".

Execution Steps

1. Open a terminal in the project directory.

2. Compile the program using:
   
   gcc insertion_sort.c -o insertion_sort

3. Run the program:
   
   ./insertion_sort
   
   On Windows, execute:
   
   insertion_sort.exe

4. Enter the number of elements.

5. Enter each array element.

6. View the sorted output.

5. Sample Input

Enter number of elements: 6
Enter the elements:
64
25
12
22
11
90

6. Sample Output

Sorted Array:
11 12 22 25 64 90

7. Time Complexity Analysis

Let "n" represent the number of elements in the array.

Case| Big-O| Big-Theta| Big-Omega
Best Case| O(n)| Θ(n)| Ω(n)
Average Case| O(n²)| Θ(n²)| Ω(n²)
Worst Case| O(n²)| Θ(n²)| Ω(n²)

Best Case

- Occurs when the array is already sorted.
- The "while" loop condition fails immediately for each element.
- Only one comparison per element is required.

Time Complexity: Θ(n)

Average Case

- Occurs when the elements are in random order.
- Elements may need to be shifted to the right to insert each key correctly.
- The number of operations grows quadratically.

Time Complexity: Θ(n²)

Worst Case

- Occurs when the array is sorted in reverse order.
- Each element must be compared with and shifted past the previous elements.
- The number of operations is proportional to (n^2).

Time Complexity: Θ(n²)

8. Space Complexity Analysis

- The algorithm uses a constant number of extra variables: "i", "j", and "key".
- It sorts the original array without creating another array.
- The additional memory required does not increase with the input size.

Auxiliary Space Complexity: O(1)

9. Advantages

- Simple to implement and understand.
- Efficient for small datasets.
- Stable sorting algorithm.
- In-place sorting algorithm.
- Performs efficiently when the array is already or nearly sorted.

10. Disadvantages

- Inefficient for large datasets.
- Average-case time complexity is O(n²).
- Worst-case time complexity is O(n²).

11. Course Outcome

CO1 – Analyze any given algorithm and express its time and space complexities using asymptotic notations.

This implementation demonstrates the analysis of Insertion Sort using Big-O, Big-Theta, and Big-Omega notations, along with auxiliary space complexity.