---
title: Arrays
teaching: 30
exercises: 0
questions:
- "How can I access subsets of data?"
- "How can I operate matrices?"
objectives:
- "Select individual values and subsections from data."
keypoints:
- "`M(row, column)` indices are used to select data points"
- "`:` is used to take slices of data"
---

We have talked about how Matlab stores all data in matrices. Let's learn how to subset data in matrices, and to operate with matrices. 

Unlike in other programming languages, Matlab does not require you to declare the array or define its size. Actually, it is possible to resize arrays in Matlab when needed. 

# Matrix indexing

There are three ways of accessing the elements of a matrix with Matlab. 
* Indexing with two subscripts: using two subscripts by giving the (row, column) coordinates. 
* Linear indexing: using only one index for each element of the matrix.
* Logical indexing: using an array the same size as the original array, with 0 (do not select) and 1 (do select). 

Let's create an example array using the "magic" function.

~~~
>> M = magic(8)
~~~
{: .language-matlab}

~~~
M =

    16     2     3    13
     5    11    10     8
     9     7     6    12
     4    14    15     1
~~~
{: .output}

## Indexing with two subscripts

We want to access a single value from the matrix. For example, number 15 which is in row 4 and column 3. The element can be selected providing the index in parenthesis.

~~~
>> M(4,3)
~~~
{: .language-matlab}

~~~
ans =

    15
~~~
{: .output}

Now we want to select a whole row, row 2. The colon notation `:` in Matlab selects a range. 

~~~
>> M(2,1:4)
~~~
{: .language-matlab}

~~~
ans =

     5    11    10     8
~~~
{: .output}

Instead of using the number 4, for which we need to remember that the matrix has 4 columns, we can use the `end` operator that refers to the last item. So,

~~~
>> M(2,1:end)
~~~
{: .language-matlab}

~~~
ans =

     5    11    10     8
~~~
{: .output}

A single : in a subscript position is shorthand notation for 1:end and is often used to select entire rows or columns:

~~~
>> M(2,:)
~~~
{: .language-matlab}

~~~
ans =

     5    11    10     8
~~~
{: .output}

To select a column we would do

~~~
>> M(:,4)
~~~
{: .language-matlab}

~~~
ans =

    13
     8
    12
     1
~~~
{: .output}


## Vector indexing

We can also refer to the items in a matrix by using only one index. In this case Matlab is treating the array as if the elements in the Matrix were strung out in a long column vector, by going down the columns consecutively, as in:


~~~
16
5
9
4
2
11
7
14
3
10
...
~~~
{: .language-matlab}




## Linear indexing

## Logical indexing

# Matrix operations


NOTE: explanations and figures of this lesson have been taken from the [Matrix Indexing in Matlab article](https://www.mathworks.com/company/newsletters/articles/matrix-indexing-in-matlab.html)
