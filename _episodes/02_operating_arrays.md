---
title: Arrays
teaching: 30
exercises: 0
questions:
- "How can I access subsets of data?"
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

If we go back to our inflammation data we can select the inflammation of the first patient over the 40 days of treatment by selecting

~~~
>> first_patient = patient_data(1,:);
~~~
{: .language-matlab}

And we can select the inflammation of all patients on day 19 by doing
~~~
>> inflammation_day_19 = patient_data(:,19);
~~~
{: .language-matlab}

## Linear indexing

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

So, the ninth element in that array will be the number 3.

~~~
>> M(9)
~~~
{: .language-matlab}

~~~
ans =

     3
~~~
{: .output}

We can use a vector of indices to select elements in a matrix:

~~~
>> M([5,8,16])
~~~
{: .language-matlab}

~~~
ans =

     2    14     1
~~~
{: .output}

A useful function that uses linear indexing is the function `find`. If we want to find the elements of the array that are larger than, say, 10, we will do

~~~
>> idx_largerthanten = find(M>10)
~~~
{: .language-matlab}

~~~
idx_largerthanten =

     1
     6
     8
    12
    13
    15
~~~
{: .output}

largerthanten is storing the linear indices of M that correspond to values larger than 10. And to see which values are these,

~~~
>> M(idx_largerthanten)
~~~
{: .language-matlab}

~~~
ans =

    16
    11
    14
    15
    13
    12
~~~
{: .output}

## Logical indexing

Logical indexing is done by having an array of the same size as the array we are considering, that is a logical array. This means that the array has only zeroes and ones. For example, many Matlab functions that start with *is* return logical arrays. 

For example, if we wanted to find the prime values in array M we would use the `prime` function.

~~~
>> primeM = isprime(M)
~~~
{: .language-matlab}

~~~
primeM =

  4×4 logical array

   0   1   1   1
   1   1   0   0
   0   1   0   0
   0   0   0   0
~~~
{: .output}

And we can operate using this arrays. We can, for example, substitute all the prime numbers with the number 2.

~~~
>> M(primeM) = 2
~~~
{: .language-matlab}

~~~
M =

    16     2     2     2
     2     2    10     8
     9     2     6    12
     4    14    15     1
~~~
{: .output}

Logical arrays can be created using logical operators. When the condition is true, a 1 will appear. Whe the condition is not true, the corresponding element of the array will be a zero. For example, to select the elements smaller than five:

~~~
>> logic_smallerthanfive = M<5
~~~
{: .language-matlab}

~~~
logic_smallerthanfive =

  4×4 logical array

   0   1   1   1
   1   1   0   0
   0   1   0   0
   1   0   0   1
~~~
{: .output}


NOTE: explanations and figures of this lesson have been taken from the [Matrix Indexing in Matlab article](https://www.mathworks.com/company/newsletters/articles/matrix-indexing-in-matlab.html)
