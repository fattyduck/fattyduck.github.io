---
layout: post
title:  "Basic Algorithms: Time Complexity"
date:   2017-03-17 02:46:41 +0000
---


What is algorithms and what does it have to do with programming? According to the omnipotent Wikipedia, an algorithm is a self-contained sequence of actions to be performed. Algorithms are generally accounted for completeness and optimization. Completeness means how well a certain algorithm addresses a problem and optimization means how efficiently can a problem be solved. Optimization or efficiency of an algorithm in programming are being rated by time and space complexities. Space complexity are the pointing to memory tax (RAM usage), while time complexity refers to iterations necessary (CPU usage).

Computer scientist came up with Big Oh Notation, Omega Omega Notation, and Theta Notation to explain time complexity of an algorithm. Big Oh Notation represents the worst case scenario.  Omega Notation represents the best case scenario. Theta Notation represents the average case scenario. Below are 4 algorithms to explain time complexity:

**Binary Search: Log(n)**

Basically Binary Search, requires a sorted list of values where you cut the list in half until you found your value. The Big Oh Notation (worst case scenario) is Log(n) which means Logarithm of the size of the list. In computer science, Binary Logarithm, the logarithm with a base of two is being used. To find find the Big Oh Notation for the list, you would use the calculator and type in* log(n)/log(2)* as most calculators have log with base of ten as default. Note: Logarithm of n with a base of two can be seen as opposite of 2 to the power of n.


**Merge Sort: n Log(n)**

In Merge Sort, generally you would split the list in half until you have a set of individual list components then compare and merge two in order at a time until you have an sorted list. All 3 Notation of Merge Sort is n log(n) with means the binary logarithm of n to the power of n. To find the total iteration of Merge Sort, you would type into the calculator *log(n^n)/log(2)*. 

**Linear Search: n**

Linear Search is more than probably the first search algorithm that everyone used. It basically means looking into the list one by one until value desired is found. The big Oh Notation for Linear search is n, which means,  worst case scenario is the value desired is the last thing in list you look at. Linear Search will never beat Binary Search in Time Complexity but it has its own merits. Firstly, it does not require the list to be sorted and there is less space complexity. Note: Assuming you are using Merge Sort, you can compare Linear Search and Binary Search by typing *n - log(n^n)/log(2) + log(n)/log(2)* into the calculator.

**Bubble Sort: n^2**

Bubble Sort is is comparing 2 values in a list from beginning to end over and over again for the size of the list. Like Merge Sort all three notations are likely to be the same. The reason, I said likely is because there are 3 different ways to do the Bubble Sort. The three ways range from n^2 to n^2-n to n + n. I will further explain the three ways to Bubble Sort in the future 
