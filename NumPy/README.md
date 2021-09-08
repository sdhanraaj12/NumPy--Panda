# NumPy
<p align="center"><image src="https://miro.medium.com/max/1400/1*cyXCE-JcBelTyrK-58w6_Q.png"></p>
  
## Introduction to NumPy
  NumPy, an acronym for the term ‘Numerical Python’, is a library in Python which is used extensively for efficient mathematical computing. This library allows users to store large amounts of data using less memory and perform extensive operations efficiently. It provides optimised and simpler functionalities to perform aforementioned operations using homogenous, one-dimensional and multidimensional arrays.

 

before delving deep into the concept of NumPy arrays, it is important to note that Python lists can very well perform all the actions that NumPy arrays perform; it is simply the fact that NumPy arrays are faster and more convenient than lists when it comes to extensive computations, which make them extremely useful, especially when you are working with large amounts of data.
  
  
## Basics of NumPy

The basic data structure of NumPy is an array. A NumPy array is a collection of values stored together, similar to a list. 

The key advantage of using NumPy arrays over lists is that arrays allow you to operate over the entire data, unlike lists. However, in terms of structure, NumPy arrays are extremely similar to lists. If you try to run the print() command over a NumPy array, then you will get the following output:

[element_1  element_2  element_3…]

The only difference between a NumPy array and a list is that the elements in the NumPy array are separated by a space instead of a comma. Hence, this is an aesthetic feature that differentiates a list and a NumPy array.

Another feature of NumPy arrays is that they are homogeneous in nature. By homogenous, we mean that all the elements in a NumPy array have to be of the same data type, which could be an integer, float, string, etc.
  
[refrence ipynb file 1](https://github.com/sdhanraaj12/NumPy-Panda/blob/master/NumPy/1.ipynb "1")

## Operations Over 1-D Arrays
  
[refrence ipynb file 2](https://github.com/sdhanraaj12/NumPy-Panda/blob/master/NumPy/2.ipynb)
  
> Q1. Extracting Elements from Array
>> Description
>> From a given array, extract all the elements which are greater than 'm' and less than 'n'. Note: 'm' and 'n' are integer values provided as input.
>> Input format:
>> A list of integers on line one
>> Integer 'm' on line two
>> Integer 'n' on line three
>> Output format:
>> 1-D array containing integers greater than 'm' and smaller than 'n'.
```python
import ast 
input_list=ast.literal_eval(input())
m=int(input())
n=int(input())

import numpy as np
array_1 = np.array(input_list)#start writing your code from here

final_array = array_1 [(array_1 > m) & (array_1 < n)]#start writing your code from here

print(final_array)
```
[practice ipynb file 1](https://github.com/sdhanraaj12/NumPy-Panda/blob/master/NumPy/3.ipynb)                                                     

## Multidimensional Arrays
                                                           
[refrence ipynb file 4](https://github.com/sdhanraaj12/NumPy-Panda/blob/master/NumPy/4.ipynb)                                                     
                                                           
NumPy arrays have certain features that help in analysing multidimensional arrays. Some features are as follows:

shape: It represents the shape of an array as the number of elements in each dimension.
ndim: It represents the number of dimensions of an array. For a 2D array, ndim = 2.
Similar to 1D arrays, nD arrays can also operate on individual elements without using list comprehensions or loops   
                                                           
[bradcasting further details](https://numpy.org/doc/stable/user/basics.broadcasting.html)

In NumPy, the dimension is called axis. In NumPy terminology, for 2-D arrays:

axis = 0 - refers to the rows
axis = 1 - refers to the columns
