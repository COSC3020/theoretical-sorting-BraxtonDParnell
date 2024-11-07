# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.


I would try sorting large amounts of data with each different iteration
growing in a linear amount each time. If the implementation is as they say
it is, then the runtime should also be growing linearly. Then, comparing these 
tests to quicksort and other sorting algorithms should help me decide if it's working 
as advertised. If so, it should run faster for large datasets than these other algorithms. 

I would be hardpressed to believe that this would be true. The fastest way we know to compare elements
to other elements is O(nlogn). With O(n), all we can do is look at each element in a data set. It would
be impossible to do anything additional to the dataset in O(n) time. For sorting algorithms like bucket sort,
we can achieve O(n). However, this requires us to have knowledge about the dataset or to only care about 
sorting it to a certain extent. In this case, X's algorithm is supposed to be general use, so it cannot be used
in this way.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
