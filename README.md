# Data-Structures-Complexity-and-Algorithms
Analyzing Data Structures

- in math, a matrix is a representations of numbers, symbols, or expresssions (in 2d)
- in Python, we can create a data structure that has values in rows and columns (kind of like a table) by using list within a list
- rows (count vertically)
- columns (count horizontally) 
- can access numbers just like how you would in a list

Example:
matrix_A = [[1,2,3,4],[5,6,7,8]]
print('Row 1: %s' % matrix_A[0])
print('Value at Row 2 Column 2: %s' % matrix_A[1][1])

Matrix is like a fancy list with the following rules:
- indexing still starts at zero here
- all rows are required to have the same number of values
- all columns must have the same number of values

List comprehesion:

- a more concise way of writing code compared to how we have been doing it before

OLD method:
squares = []
for i in range(10):
  squares.append(i**2)
  
print('our result: %s' % squares)

characteristics of list comprehension:
- a square bracket containing an expression that describes the list
- one or more for clase to explain its members 
- then if clauses if needed

LIST COMPREHENSION:

squares = [i**2 for i in range(10)] #the expression that describes the list, for statement included
print('our new result : %s' % squares) 
- program prints the squares of all numbers starting at 1
* in this case no if statement needed

list comprehension (example2):

vec = [[1,2,3],[4,5,6],[7,8,9]]

result = [value for row in vec for value in row]
print('Vec as a single list of values: %s' % result)
- Vec as a single list of values: [1,2,3,4,5,6,7,8,9]

Map and Filter in Python 3

Formatting:

map(function_name, sequence)

