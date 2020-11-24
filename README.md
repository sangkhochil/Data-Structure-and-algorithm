# Data-Structure-and-algorithm

### Types of Asymptotic Notations
We use three types of asymptotic notations to represent the growth of any algorithm, as input increases:

- Big Theta (Θ)
- Big Oh(O)
- Big Omega (Ω)

#### Tight Bounds: Theta (average case)
When we say tight bounds, we mean that the time compexity represented by the Big-Θ notation is like the average value or range within which the actual time of execution of the algorithm will be.

For example, if for some algorithm the time complexity is represented by the expression 3n2 + 5n, and we use the Big-Θ notation to represent this, then the time complexity would be Θ(n2), 
ignoring the constant coefficient and removing the insignificant part, which is 5n.

Here, in the example above, complexity of Θ(n2) means, that the avaerage time for any input n will remain in between, k1 * n2 and k2 * n2, where k1, k2 are two constants, therby tightly binding the expression rpresenting the growth of the algorithm.

![alt text](https://github.com/sangkhochil/java/blob/main/Resources/asymptotic_notation.png?raw=true)

#### Upper Bounds: Big-O (Worst Case)
This notation is known as the upper bound of the algorithm, or a Worst Case of an algorithm.

It tells us that a certain function will never exceed a specified time for any value of input n.

The question is why we need this representation when we already have the big-Θ notation, which represents the tightly bound running time for any algorithm. Let's take a small example to understand this.

Consider Linear Search algorithm, in which we traverse an array elements, one by one to search a given number.

In Worst case, starting from the front of the array, we find the element or number we are searching for at the end, which will lead to a time complexity of n, where n represents the number of total elements.

But it can happen, that the element that we are searching for is the first element of the array, in which case the time complexity will be 1.

Now in this case, saying that the big-Θ or tight bound time complexity for Linear search is Θ(n), will mean that the time required will always be related to n, as this is the right way to represent the average time complexity, but when we use the big-O notation, we mean to say that the time complexity is O(n), which means that the time complexity will never exceed n, defining the upper bound, hence saying that it can be less than or equal to n, which is the correct representation.

This is the reason, most of the time you will see Big-O notation being used to represent the time complexity of any algorithm, because it makes more sense.

#### Lower Bounds: Omega (best case)
Big Omega notation is used to define the lower bound of any algorithm or we can say the best case of any algorithm.

This always indicates the minimum time required for any algorithm for all input values, therefore the best case of any algorithm.

In simple words, when we represent a time complexity for any algorithm in the form of big-Ω, we mean that the algorithm will take atleast this much time to cmplete it's execution. It can definitely take more time than this too.

#### Bubble Sort
- Worst Case Time Complexity [ Big-O ]: O(n2)
- Best Case Time Complexity [Big-omega]: O(n)
- Average Time Complexity [Big-theta]: O(n2)
- Space Complexity: O(1)

#### Selection Sort
- Worst Case Time Complexity [ Big-O ]: O(n2)
- Best Case Time Complexity [Big-omega]: O(n2)
- Average Time Complexity [Big-theta]: O(n2)
- Space Complexity: O(1)

#### Insertion Sort
- Worst Case Time Complexity [ Big-O ]: O(n2)
- Best Case Time Complexity [Big-omega]: O(n)
- Average Time Complexity [Big-theta]: O(n2)
- Space Complexity: O(1)

#### Merge Sort
- Worst Case Time Complexity [ Big-O ]: O(n*log n)
- Best Case Time Complexity [Big-omega]: O(n*log n)
- Average Time Complexity [Big-theta]: O(n*log n)
- Space Complexity: O(n)

#### Quick Sort
- Worst Case Time Complexity [ Big-O ]: O(n2)
- Best Case Time Complexity [Big-omega]: O(n*log n)
- Average Time Complexity [Big-theta]: O(n*log n)
- Space Complexity: O(n*log n)

#### Heap Sort
- Worst Case Time Complexity: O(n*log n)
- Best Case Time Complexity: O(n*log n)
- Average Time Complexity: O(n*log n)
- Space Complexity : O(1)

#### Reference's ####
1. https://www.studytonight.com/