# Hashing and Randomized Algorithms

## 1. What is Hashing?

Hashing is a technique for mapping data of arbitrary size (often a key) to a fixed-size value. The hash function takes an input and produces a hash code that is used to index into a hash table. Hashing is widely used in many fields, including databases, cryptography, and data structures.

### Hash Function
A hash function is a mathematical function that takes an input (or 'key') and returns a fixed-size value, often an integer. The goal of a hash function is to distribute the input keys evenly across the hash table to minimize collisions (i.e., when two keys hash to the same value).

```python
def simple_hash(key, size):
    return sum(ord(char) for char in key) % size
