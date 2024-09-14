# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
  - Asymptotic analysis ignores constant factors and lower order terms.
  - Hardware is anot often considered while conducting asymtotic analysis
  - The use of loose bound during analysis. This could lead to an algorthim being much faster
    then the analysis suggests. 

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.
  - We know that to search 1,000 elements it takes 5 seconds.
  - We also know from lecture that Binary Search has a time complexity of $O(\log(n))$
  - Knowing this we can determine that the search time for 1,000 elements is related to $\log(1,000)$
  - This means we can assume the search time for 10,000 elements is $\log(10,000)$
  - since we can see the difference in the search time for each number of elements we can use the difference to determine the time it takes to search for a value out of 10,000 using the time it takes to find a element out of 1,000.
  - $\frac{\log(1,000)}{\log(10,000)} = \frac{13.3}{10} \approx 1.33$
  - $1.33 \cdot 5 = 6.65$ seconds

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.
