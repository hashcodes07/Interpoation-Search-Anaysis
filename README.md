# Interpoation-Search-Anaysis
This is an analysis of a searching algorithm  called Interpolation Search. 
It gives time complexity analysis and comparison with Binary Search Algorithm

Analysis of Interpolation Search
Overview
This project analyzes the performance and behavior of the Interpolation Search algorithm and compares its efficiency under different data distributions.

Objective
Implement Interpolation Search
Measure execution time
Compare with Binary Search
Observe best, average, and worst cases
What is Interpolation Search?



Algorithm
1. Accept two inputs from the user:
o Number of elements to generate.
o Search key.
2. Automatically generate a uniformly distributed sorted array.
3. Perform Interpolation Search to locate the search key.
4. Measure and display the execution time.
5. Display the time complexity and space complexity.
6. Plot a line graph showing the theoretical time complexity growth of Interpolation
Search for different input sizes.

Time Complexity
| Case             | Time Complexity  | Explanation                                                                 |
| ---------------- | ---------------- | --------------------------------------------------------------------------- |
| **Best Case**    | **O(1)**         | Element is found at the estimated position immediately                      |
| **Average Case** | **O(log log n)** | Works efficiently when data is uniformly distributed                        |
| **Worst Case**   | **O(n)**         | Happens when data is unevenly distributed or interpolation estimates poorly |

Results

The analysis shows that Interpolation Search performs efficiently for sorted and uniformly distributed datasets by estimating the likely position of the target element instead of repeatedly dividing the array into halves.

Time Complexity Comparison
Algorithm	Best Case	Average Case	Worst Case
Interpolation Search	O(1)	O(log log n)	O(n)
Binary Search	O(1)	O(log n)	O(log n)

From the observations:

Interpolation Search outperformed Binary Search when the dataset values were distributed uniformly.
The estimated index reduced the number of comparisons, leading to lower execution time.
For irregular or non-uniform datasets, Interpolation Search lost efficiency and in some cases approached linear performance O(n).
Binary Search remained more stable because its performance is independent of data distribution.
| Algorithm            | Space Complexity |
| -------------------- | ---------------- |
| Interpolation Search | O(1)             |
| Binary Search        | O(1)             |


Both algorithms require constant extra memory, making them space-efficient.

Final Observation

Interpolation Search can be considered faster than Binary Search under ideal conditions due to its O(log log n) average complexity. However, Binary Search provides more consistent performance across different datasets. Therefore, Interpolation Search is most suitable when the input data is sorted and approximately uniformly distributed.


Conclusion

This project analyzed the performance of the Interpolation Search algorithm and its behavior across different input cases. The results show that Interpolation Search can achieve very fast search performance with an average time complexity of O(log log n) when the data is sorted and uniformly distributed.

However, its efficiency depends heavily on the distribution of values. When the data is unevenly distributed, the estimated positions become less accurate and performance may degrade to O(n) in the worst case.

Overall, Interpolation Search is an effective alternative to Binary Search for suitable datasets, but its advantages are reduced when data distribution is irregular. Choosing the appropriate search algorithm depends on the characteristics of the input data and the required performance.
