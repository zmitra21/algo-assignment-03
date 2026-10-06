# CMPS 2200 Assignment 3
## Answers

**Name:**Zack Mitra


Place all written answers from `assignment-03.md` here for easier grading.


**1: Searching Unsorted Lists**

- **1b.** Work and span of `isearch` implementation
W(n) = W(n-1) + O(1) is in O(n)
S(n) = S(n-1) + O(1) is in O(n)

- **1d.** Work and span of `rsearch` implementation
W(n) = 2W(n/2) + O(1) is in O(n)
S(n) = S(n/2) + O(1) is in O(log(n))

- **1e.** Work and span of `rsearch` using `ureduce`
W(n) = W(n/3) + W(2n/3) + O(1) is in O(n)
S(n) = S(2n/3) + O(1) is in O(log(n))

**3: Parenthesis Matching**

- **3b.** Recurrences and Big-Oh solutions for `parens_match_iterative`
W(n) = W(n-1) + O(1) is in O(n)
S(n) = S(n-1) + O(1) is in O(n)

- **3d.** Work and Span for `parens_match_scan`
        O(n)    O(n)        O(n)
W(n) = Wmap(n) + Wscan(n) + Wreduce(n) + O(1) is in O(n)
        O(1)    O(log(n))   O(log(n))  
S(n) = Smap(n) + Sscan(n) + Sreduce(n) + O(1) is in O(log(n))

- **3f.** Recurrences and Big-Oh solutions for `parens_match_dc_helper`
left = n/2 ; right = n/2

W(n) = 2W(n/2) + O(1)
W(n) is in O(n)

S(n) = S(n/2) + O(1)
S(n) = O(log(n))