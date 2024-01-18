# ST2195 Assignment 5

This repository is for the fifth assignment of the ST2195 course. The assignment involves debugging a Python script and pushing the corrected code to this GitHub repository.

## Assignment Details

The assignment consists of the following steps:

1. Commit and push the provided Python code as a file named "foo.py".
2. Find and fix all the bugs in the code. Each fixed bug is worth 1 point.
3. Update "foo.py" by committing and pushing the revisions.

## Python Script

The provided Python script includes a function `is_divisible_by_k(x, k)` that checks whether `x` is divisible by `k`. The script then attempts to store all integers that are multiples of 2, 5, or 7 and are less than or equal to 1000 (excluding duplicates). Finally, it sums all these integers.

Here is the original script:

```python
def is_divisible_by_k(x, k): '''
    Checks whether x is divisible by k.
'''
    assert x%k == 0

'''
Store all the integers that are multiples of 2 or 5 or 7 that are lower or equal to 1000 (excluding doubles)
'''
x = ()
for i in range(1000):
    if (is_divisible_by_k(x, 2) & is_divisible_by_k(x, 3)) | is_divisible_by_k(x, 7):
        x.append(i)

'''
Sum all the integers that are multiples of 2 or 5 or 7 that are lower or equal to 1000 (excluding doubles)
'''
sum(x)
