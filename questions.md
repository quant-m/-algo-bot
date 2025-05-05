# Concept Questions – Hashing and Randomized Algorithms

## 1. What is the average-case time complexity of searching in a hash table?
**Answer:** O(1), assuming a good hash function and no collisions.

## 2. What is the primary benefit of using randomized algorithms in sorting?
**Answer:** Randomized algorithms, like Randomized QuickSort, avoid worst-case performance (O(n^2)) in sorted or reverse-sorted inputs by selecting a random pivot.

## 3. What is the difference between Monte Carlo and Las Vegas algorithms?
**Answer:** 
- Monte Carlo algorithms may produce incorrect results but have bounded runtime.
- Las Vegas algorithms always produce the correct result but may take a random amount of time.

## 4. Why is universal hashing important in hash tables?
**Answer:** Universal hashing minimizes the likelihood of collisions, even in the worst case, by randomly choosing a hash function from a family of functions.

## 5. What is a Hash Set, and how is it different from a hash table?
**Answer:** A Hash Set is a collection of unique elements implemented using a hash table, while a hash table stores key-value pairs.
