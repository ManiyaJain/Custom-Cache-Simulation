# Custom Cache Simulation

A simple Java implementation that demonstrates how an **LRU (Least Recently Used) Cache** works internally.  
This project simulates custom cache behavior using **HashMap** and **Deque (LinkedList)** to maintain insertion order and track recently used keys.

---

## 🚀 Features
- Custom implementation of an **LRU Cache** without using built-in LinkedHashMap.
- Efficient **O(1)** operations for:
  - `get(key)`
  - `put(key, value)`
- Automatic eviction of **least recently used (LRU)** entry when capacity is full.
- Clear visualization of cache state using a `display()` method.
- Generic implementation using `<K, V>` types.

---

## 🧠 How It Works

### ✔ HashMap  
Stores key-value pairs for **constant time lookup**.

### ✔ Deque (LinkedList)  
Maintains usage order:  
- **Front** → most recently used  
- **Back** → least recently used  

### ✔ Cache Mechanics
- `get(key)` → refreshes the key by moving it to the front.
- `put(key, value)`:
  - If key exists → update + refresh.
  - If cache is full → evict least recently used key.
  - Insert the new key at the front.

---

## 🎯 What You Learn

- How LRU caching works internally.
- Achieving O(1) operations using HashMap + Deque.
- Designing clean and generic Java classes.
- Managing eviction policies manually.

---

## 📘 Future Enhancements

- LFU Cache implementation
- Time-based eviction
- JUnit test suite
- GUI-based visualization

---

## ❤️ Contributions

Feel free to fork, improve, and submit PRs.
