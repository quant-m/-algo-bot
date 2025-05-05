
# Concept Snippets – Hashing and Randomized Algorithms

## 1. Hash Function
A hash function is a function that maps data (key) to a fixed-size value (hash code). It should be fast to compute and distribute keys evenly across the hash table.

## 2. Hash Table
A hash table is a data structure that stores key-value pairs. It uses a hash function to map keys to indices in an array, providing fast access (O(1) average case).

## 3. Collision Resolution
When two keys hash to the same index, it’s called a collision. Techniques to resolve collisions include chaining (linked lists) and open addressing (probing).

## 4. Universal Hashing
Universal hashing involves selecting a hash function randomly from a family of functions. This reduces the chance of collisions, even in adversarial cases.

## 5. Randomized QuickSort
A variant of QuickSort where the pivot is chosen randomly, ensuring that the average time complexity is O(n log n) and reducing the likelihood of worst-case O(n^2) time.

## 6. Monte Carlo Algorithm
A Monte Carlo algorithm is a randomized algorithm that might produce an incorrect result, but the probability of failure is small. It has a fixed runtime.

## 7. Las Vegas Algorithm
A Las Vegas algorithm always produces a correct result, but its runtime may vary. Examples include Randomized QuickSort and some primality tests.

## 8. Hash Set
A hash set is a collection of unique elements that is implemented using a hash table. It provides O(1) time complexity for add, remove, and check operations on average.

## 9. Bloom Filter
A Bloom filter is a probabilistic data structure used to test whether an element is a member of a set. It allows false positives but never false negatives.

## 10. Hashing in Cryptography
Cryptographic hash functions, such as SHA-256, are designed to be one-way functions that map data to a fixed-length hash, providing data integrity and security.
