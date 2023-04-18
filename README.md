<h1 align="center"> IT-315 Lab-7</h1>
<!-- <h1 align="center"> </h1> -->

### Name: Harsh Makwana
### Student ID: 202001264

# **Section A**
<h3>P1:</h3>

| Tester Action and Input Data      | Expected Outcome |
|-----------------------------------|------------------|
|                                   |                  |
| Equivalence Partitioning          |                  |
| When value is found:              |                  |
| [1, 2, 3, 4, 5], 3                | 2                |
| When value is not found:          |                  |
| [2, 4, 6, 8], 5                   | -1               |
| When a variable is non-integer:   |                  |
| [a, 3, 5, 7], 4                   | Invalid          |
| When an integer is not in range:  |                  |
| [1, 3, 5, INT_MAX+2], 7           | Invalid          |
| [1, 3, 5, 7], INT_MAX+12          | Invalid          |
| [INT_MIN-21, 1, 3, 5], 7          | Invalid          |
| [1, 3, 5, 7], INT_MIN-12          | Invalid          |
| When array is empty:              |                  |
| [], 5                             | -1               |
|                                   |                  |
| Boundary Value Analysis:          |                  |
| When value is found:              |                  |
| [5, 10, 15, 20, 25], 5            | 0                |
| [5, 10, 15, 20, 25], 25           | 4                |
| When array is empty:              |                  |
| [], 5                             | -1               |
| When value is not found:          |                  |
| [3, 7, 9, 11], 10                 | -1               |
| When an integer is not in range:  |                  |
| [1, 3, 5, INT_MAX+1], 7           | Invalid          |
| [1, 3, 5, 7], INT_MAX+1           | Invalid          |
| [INT_MIN-1, 1, 3, 5], 7           | Invalid          |
| [1, 3, 5, 7], INT_MIN-1           | Invalid          |

<h2>P2:</h2>

| Tester Action and Input Data        | Expected Outcome |
|-------------------------------------|------------------|
|                                     |                  |
| Equivalence Partitioning            |                  |
| When integer is found:              |                  |
| [5, 5, 6, 7, 8, 5], 5               | 3                |
| When integer is not found:          |                  |
| [2, 4, 6, 8], 5                     | 0                |
| When a variable is non-integer:     |                  |
| [a, 3, 5, 7], 4                     | Invalid          |
| When an integer is not in range:    |                  |
| [1, 3, 5, INT_MAX+1], 7             | Invalid          |
| [1, 3, 5, 7], INT_MAX+1             | Invalid          |
| [INT_MIN-1, 1, 3, 5], 7             | Invalid          |
| [1, 3, 5, 7], INT_MIN-1             | Invalid          |
| When array is empty:                |                  |
| [], 5                               | -1               |
|                                     |                  |
| Boundary Value Analysis:            |                  |
| When array is empty:                |                  |
| [], 5                               | -1               |
| When value is found once:           |                  |
| [5, 10, 15, 20, 25], 5              | 1                |
| When value is found multiple times: |                  |
| [5, 10, 15, 20, 25], 5              | 1                |
| [5], 5                              | 1                |
| When integer is not found:          |                  |
| [12, 24, 36, 48], 5                 | 0                |

<h2>P3:</h2>

| Tester Action and Input Data        | Expected Outcome |
|-------------------------------------|------------------|
|                                     |                  |
| Equivalence Partitioning            |                  |
| When value is found:                |                  |
| [1, 2, 3, 4, 5], 3                  | 2                |
| When value is not found:            |                  |
| [2, 4, 6, 8], 5                     | -1               |
| When a variable is non-integer:     |                  |
| [a, 3, 5, 7], 4                     | Invalid          |
| When an integer is not in range:    |                  |
| [1, 3, 5, INT_MAX+2], 7             | Invalid          |
| [1, 3, 5, 7], INT_MAX+12            | Invalid          |
| [INT_MIN-21, 1, 3, 5], 7            | Invalid          |
| [1, 3, 5, 7], INT_MIN-12            | Invalid          |
| When array is empty:                |                  |
| [], 5                               | -1               |
|                                     |                  |
| Boundary Value Analysis:            |                  |
| When value is found:                |                  |
| [5, 10, 15, 20, 25], 5              | 0                |
| [5, 10, 15, 20, 25], 25             | 4                |
| When array is empty:                |                  |
| [], 5                               | -1               |
| When value is not found:            |                  |
| [3, 7, 9, 11], 10                   | -1               |
| When an integer is not in range:    |                  |
| [1, 3, 5, INT_MAX+1], 7             | Invalid          |
| [1, 3, 5, 7], INT_MAX+1             | Invalid          |
| [INT_MIN-1, 1, 3, 5], 7             | Invalid          |
| [1, 3, 5, 7], INT_MIN-1             | Invalid          |
| When (length of array)>(INTMAX/2):  |                  |
| [1, 3, 5,...], 6                    | Invalid          |

<h2>P4:</h2>

| Tester Action and Input Data |     |    | Expected Outcome |
|------------------------------|-----|----|------------------|
| Equivalence Partitioning:    |     |    |                  |
| A                            | B   | C  |                  |
| 1                            | 2   | 3  | Invalid          |
| 3                            | 3   | 3  | Equilateral      |
| 6                            | 6   | 4  | Isosceles        |
| 2                            | 3   | 4  | Scalene          |
|                              |     |    |                  |
| Boundary Value Analysis:     |     |    |                  |
| A                            | B   | C  |                  |
| 1                            | 2   | 3  | Invalid          |
| 1                            | 3   | 2  | Invalid          |
| 3                            | 1   | 2  | Invalid          |
| 5                            | 5   | 5  | Equilateral      |
| 8.5                          | 8.5 | 7  | Isosceles        |
| 6                            | 4   | 6  | Isosceles        |
| 3                            | 5   | 5  | Isosceles        |
| 15                           | 32  | 34 | Scalene          |

<h2>P5:</h2>

| Tester Action and Input Data |          | Expected Outcome |
|------------------------------|----------|------------------|
| Equivalence Partitioning:    |          |                  |
| s1                           | s2       |                  |
| ""                           | ""       | True             |
| ""                           | "hello"  | True             |
| "Mo"                         | "Motion" | True             |
| "gs"                         | "Songs"  | False            |
| "abababa"                    | "ab"     | False            |
|                              |          |                  |
| Boundary Value Analysis:     |          |                  |
| s1                           | s2       |                  |
| ""                           | ""       | True             |
| ""                           | "music"  | True             |
| "ft"                         | "Lift"   | False            |
| "cdcdcdc"                    | "cd"     | False            |

<h2>P6:</h2>

Program 6:

Equivalence classes for the system

EC1: All sides are positive, real numbers.
EC2: One or more sides are negative or zero.
EC3: The sum of the lengths of any two sides is less than or equal to the length of the remaining side (impossible lengths).
EC4:  The sum of the lengths of any two sides is greater than the length of the remaining side (possible lengths).


b) Test cases to cover equivalence classes

TC1 (EC1): A=3, B=4, C=5 (right-angled triangle)
TC2 (EC1): A=5, B=5, C=5 (equilateral triangle)
TC3 (EC1): A=5, B=6, C=7 (scalene triangle)
TC4 (EC1): A=5, B=5, C=7 (isosceles triangle)
TC5 (EC2): A=-2, B=4, C=5 (invalid input)
TC6 (EC2): A=0, B=4, C=5 (invalid input)

c) Test cases for boundary condition A+B>C

TC7 (EC4): A=4, B=3, C=6 (sum of A and B > C)


d) Test case for boundary condition A=C

TC8 (EC4): A=5, B=6, C=5 (A equals to C)

e)Test case for the boundary condition A=B=C

TC9 (EC4): A=5, B=5, C=5 (all sides are equal)

f) Test case for the boundary condition A^2 + B^2 = C^2

TC10 (EC4): A=3, B=4, C=5 (right-angled triangle)

g) Test cases for the boundary condition of non-triangle case:

TC11 (EC3): A=2, B=2, C=4 (sum of A and B is equal to C)

h) For non-positive input, identify test points.

TP1 (EC2): A=0, B=4, C=5 (invalid input)
TP2 (EC2): A=-2, B=4, C=5 (invalid input)

The Test cases TC1 to TC10 covers all identified equivalence classes.


# **Section B**
1. **Control flow diagram:**<br>
![control-flow-diagram drawio](https://user-images.githubusercontent.com/75673068/231425222-27f0cc54-8a37-41a1-8d0f-b57b1db680a2.png)

2. **Test sets:**<br>

**a) Statement coverage test sets:** To achieve statement coverage, we need to make sure that every statement in the code is executed at least once.
<br>
* Test 1: p = empty vector
* Test 2: p = vector with one point
* Test 3: p = vector with two points with the same y component
* Test 4: p = vector with two points with different y components
* Test 5: p = vector with three or more points with different y components
* Test 6: p = vector with three or more points with the same y component

<br>

**b) Branch coverage test sets:** To achieve branch coverage, we need to make sure that every possible branch in the code is taken at least once
<br>
* Test 1: p = empty vector
* Test 2: p = vector with one point
* Test 3: p = vector with two points with the same y component
* Test 4: p = vector with two points with different y components
* Test 5: p = vector with three or more points with different y components, and none of them have the same x component
* Test 6: p = vector with three or more points with the same y component, and some of them have the same x component
* Test 7: p = vector with three or more points with the same y component, and all of them have the same x component

<br>

**c) Basic condition coverage test sets:** To achieve basic condition coverage, we need to make sure that every basic condition in the code (i.e., every Boolean subexpression) is evaluated as both true and false at least once
<br>
* Test 1: p = empty vector
* Test 2: p = vector with one point
* Test 3: p = vector with two points with the same y component, and the first point has a smaller x component
* Test 4: p = vector with two points with the same y component, and the second point has a smaller x component
* Test 5: p = vector with two points with different y components
* Test 6: p = vector with three or more points with different y components, and none of them have the same x component
* Test 7: p = vector with three or more points with the same y component, and some of them have the same x component
* Test 8: p = vector with three or more points with the same y component, and all of them have the same x component.
