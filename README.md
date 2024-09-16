# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  - Asymptotic analysis ignores constant factors and lower order terms
  - Hardware is not often considered while conducting asymtotic analysis
  - The use of loose bound during analysis. This could lead to an algorthim being much faster
    then the analysis suggests

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  - We know that to search 1,000 elements it takes 5 seconds
  - We also know that binary search has a time complexity of $O(\log(n))$
  - Knowing this we can determine that the search time for 1,000 elements is related to $\log(1,000)$
  - This means we can assume the search time for 10,000 elements is $\log(10,000)$
  - since we can see the difference in the search time for each number of elements we can use the difference to determine the time it 
    takes to search for a value out of 10,000 using the time it takes to find a element out of 1,000
  - $\frac{\log(1,000)}{\log(10,000)} = \frac{13.3}{10} = 1.33$
  - $1.33 \cdot 5 = 6.65$ seconds

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time
  - It's unlikely that an unbalanced tree alone would cause such a huge time difference from the expected 6.65 seconds to 100 seconds
  - While an unbalanced tree could increase the search time from logarithmic to linear, the change from 6.65 to 100 seconds makes me think that other factors are also envolved
  - For example, if there were multiple programs running simultaneously, or you are running this search on a different system entirely
  - The combination of an unbalanced tree and the senario which it is being run in could explain such a large difference in runtime

Add your answers to this markdown file.

## Plagiarism Acknowledgment

I Remember having difficulty with this assignment prior. I reviewed the repositroy and the comments from 
the repository https://github.com/COSC3020/theory-vs-practice-swilso59-1.git
it looked like I was not being specific enough in that there would have to be multipe causes for a time difference of that 
significants.

“I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.”
