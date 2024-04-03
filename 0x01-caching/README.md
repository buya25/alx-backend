# Project Tasks

This project consists of implementing various caching systems using Python. Each caching system is a class that inherits from a base class called `BaseCaching` and implements specific caching algorithms. The implemented caching systems are:

1. Basic Cache
2. FIFO Cache
3. LIFO Cache
4. LRU Cache
5. MRU Cache
6. LFU Cache

## Installation

Clone the GitHub repository and navigate to the appropriate directory:

```bash
git clone https://github.com/alx-backend
cd 0x01-caching
```

## Usage

### 0. Basic Cache

This caching system doesn’t have a limit and simply stores key-value pairs.

Example usage:

```python
from 0-basic_cache import BasicCache

my_cache = BasicCache()
my_cache.put("A", "Hello")
my_cache.put("B", "World")
my_cache.put("C", "Holberton")

print(my_cache.get("A"))  # Output: Hello
print(my_cache.get("B"))  # Output: World
print(my_cache.get("C"))  # Output: Holberton
print(my_cache.get("D"))  # Output: None
```

### 1. FIFO Cache

Implements a caching system using the First-In-First-Out (FIFO) algorithm.

Example usage:

```python
from 1-fifo_cache import FIFOCache

my_cache = FIFOCache()
my_cache.put("A", "Hello")
my_cache.put("B", "World")
my_cache.put("C", "Holberton")
my_cache.put("D", "School")

print(my_cache.get("A"))  # Output: None (A was discarded)
print(my_cache.get("B"))  # Output: World
print(my_cache.get("C"))  # Output: Holberton
print(my_cache.get("E"))  # Output: None (E was discarded)
```

### 2. LIFO Cache

Implements a caching system using the Last-In-First-Out (LIFO) algorithm.

Example usage:

```python
from 2-lifo_cache import LIFOCache

my_cache = LIFOCache()
my_cache.put("A", "Hello")
my_cache.put("B", "World")
my_cache.put("C", "Holberton")
my_cache.put("D", "School")

print(my_cache.get("A"))  # Output: Hello
print(my_cache.get("B"))  # Output: World
print(my_cache.get("C"))  # Output: None (C was discarded)
print(my_cache.get("E"))  # Output: None (E was discarded)
```

### 3. LRU Cache

Implements a caching system using the Least Recently Used (LRU) algorithm.

Example usage:

```python
from 3-lru_cache import LRUCache

my_cache = LRUCache()
my_cache.put("A", "Hello")
my_cache.put("B", "World")
my_cache.put("C", "Holberton")
my_cache.put("D", "School")

print(my_cache.get("B"))  # Output: World (B is now the most recently used)
print(my_cache.get("A"))  # Output: None (A was discarded)
print(my_cache.get("C"))  # Output: Holberton
```

### 4. MRU Cache

Implements a caching system using the Most Recently Used (MRU) algorithm.

Example usage:

```python
from 4-mru_cache import MRUCache

my_cache = MRUCache()
my_cache.put("A", "Hello")
my_cache.put("B", "World")
my_cache.put("C", "Holberton")
my_cache.put("D", "School")

print(my_cache.get("B"))  # Output: World (B is the most recently used)
print(my_cache.get("A"))  # Output: None (A was discarded)
print(my_cache.get("C"))  # Output: Holberton
```

### 5. LFU Cache

Implements a caching system using the Least Frequently Used (LFU) algorithm.

Example usage:

```python
from 100-lfu_cache import LFUCache

my_cache = LFUCache()
my_cache.put("A", "Hello")
my_cache.put("B", "World")
my_cache.put("C", "Holberton")
my_cache.put("D", "School")

print(my_cache.get("B"))  # Output: World
print(my_cache.get("A"))  # Output: None (A was discarded)
print(my_cache.get("C"))  # Output: Holberton
```

## Files

- `0-basic_cache.py`: Implementation of the Basic Cache class.
- `1-fifo_cache.py`: Implementation of the FIFO Cache class.
- `2-lifo_cache.py`: Implementation of the LIFO Cache class.
- `3-lru_cache.py`: Implementation of the LRU Cache class.
- `4-mru_cache.py`: Implementation of the MRU Cache class.
- `100-lfu_cache.py`: Implementation of the LFU Cache class.

## Credits

This project is part of the ALX Software Engineering curriculum. The task descriptions and example usage were provided by ALX.
