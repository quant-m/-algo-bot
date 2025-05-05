# Classic Problems – Hashing and Randomized Algorithms

## Problem 1: Two Sum
**Description:** Given an array of integers and a target sum, find the indices of two numbers that add up to the target.
**Hint:** Use a hash map to store the difference between the target and the current number.

**Solution:**
```python
def two_sum(nums, target):
    seen = {}
    for i, num in enumerate(nums):
        if target - num in seen:
            return [seen[target - num], i]
        seen[num] = i
```

## Problem 2: Randomized QuickSort

Description: Implement the Randomized QuickSort algorithm, where the pivot is chosen randomly to ensure good average performance.

Solution:

```python
def has_cycle(head):
    visited = set()
    while head:
        if head in visited:
            return True
        visited.add(head)
        head = head.next
    return False

```


## Problem 3: Detect Cycle in a Linked List

Description: Use hashing to detect a cycle in a linked list.
Hint: Use a hash set to track visited nodes.
Solution:

```python
def has_cycle(head):
    visited = set()
    while head:
        if head in visited:
            return True
        visited.add(head)
        head = head.next
    return False
```
## Problem 4: Miller-Rabin Primality Test

Description: Implement the Miller-Rabin primality test to check if a number is probably prime.
Hint: Use probabilistic witnesses to test primality.

Solution: Available in most libraries as is_probably_prime().

```python
import random

def miller_rabin(n, k=5):
    if n == 2 or n == 3:
        return True
    if n % 2 == 0:
        return False

    r, s = 0, n - 1
    while s % 2 == 0:
        r += 1
        s //= 2

    for _ in range(k):
        a = random.randint(2, n - 1)
        x = pow(a, s, n)
        if x == 1 or x == n - 1:
            continue
        for _ in range(r - 1):
            x = pow(x, 2, n)
            if x == n - 1:
                break
        else:
            return False
    return True
```

