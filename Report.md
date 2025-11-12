# Beyond Recursion Report

## Part A — Fibonacci

### Observations
**Recursive Fibonacci**
- Works but gets slow very quickly.
- Each call makes two more calls, so time grows fast (exponential).
- For large n (around 40–45), it takes several seconds.
- Uses more stack space because of many recursive calls.

**Iterative Fibonacci**
- Runs almost instantly, even for large n.
- Time grows slowly and stays very small.
- Uses a simple loop with two variables — constant memory.

**Conclusion**
Recursive Fibonacci is simple to write but very slow for big inputs.  
Iterative Fibonacci is much faster and more efficient.

---

## Part B — Linked List InsertLast

### Observations
**Iterative Version**
Trial 1: 0.033 ms, depth = 1
Trial 2: 0.033 ms, depth = 1
Trial 3: 0.032 ms, depth = 1
- Time stayed about the same each time.
- Stack depth always 1 → constant memory.
- Very fast and stable.

**Recursive Version**
Trial 1: 0.397 ms, depth = 5000
Trial 2: 0.087 ms, depth = 5001
Trial 3: 0.090 ms, depth = 5002
- Stack depth grows with the list size.
- Slower than iterative.
- Can cause StackOverflowError for very large lists.

**Conclusion**
Iterative insert runs in constant time and memory.  
Recursive insert uses more stack and is slower for big lists.

Recursion can look elegant but often uses more time and memory.  
Iteration is usually faster and safer in Java.