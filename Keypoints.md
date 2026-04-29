# 🧠 Programming Languages Overview

## 🟡 Interpreted Languages
 Code is executed line-by-line at runtime (no separate compilation step)

### 📌 Examples:
- JavaScript
- Python

### ⚡ Key Characteristics:
- Faster development (no compile step)
- Easier debugging
- Slower execution compared to compiled languages

### 🧠 Real-world Use:
- Web development (frontend/backend)
- Scripting & automation

---

## 🔵 Compiled Languages
Code is converted into machine code before execution

### 📌 Examples:
- C++
- Rust
- Java
- Go (Golang)

### ⚡ Key Characteristics:
- Faster execution
- Better performance
- Compilation required before running

### 🧠 Real-world Use:
- System programming
- Game engines
- High-performance applications



## ⚔️ Interpreted vs Compiled (Quick Comparison)

| Feature            | Interpreted 🟡        | Compiled 🔵            |
|------------------|----------------------|------------------------|
| Execution Speed   | Slower               | Faster                 |
| Development Time  | Faster               | Slower (compile step)  |
| Error Detection   | Runtime              | Compile-time           |
| Portability       | High                 | Depends on binary      |

---

## 🎯 Interview Insight

- Java is **both compiled + interpreted** (JVM concept)
- JavaScript uses **JIT (Just-In-Time Compilation)** → not purely interpreted
- Performance-critical apps → prefer compiled languages



## ❓ Follow-up Questions (Interview Traps)

- Why is Java not purely compiled?
- What is JIT compilation?
- Why is Python slower than C++?
- Can interpreted languages be faster in some cases?

---

## ⚡ Synchronous vs Asynchronous Functions


### 🟡 Synchronous (Sync)
Executes step-by-step (blocking)

- One task at a time  
- Next task waits until current finishes  
- Blocking nature  
- Simple to debug  
- Not efficient for I/O operations  

#### 📌 Example:
```js
console.log("Start");
console.log("Task 1");
console.log("Task 2");
console.log("End");
```

#### 🧾 Output:
```
Start
Task 1
Task 2
End
```

---

### 🔵 Asynchronous (Async)
Non-blocking execution

- Does not wait for task completion  
- Uses background handling (Web APIs)  
- Improves performance for I/O tasks  
- Uses callbacks, Promises, async/await  
- Execution order may differ  

#### 📌 Example:
```js
console.log("Start");

setTimeout(() => {
  console.log("Task 1");
}, 2000);

console.log("End");
```

#### 🧾 Output:
```
Start
End
Task 1
```

---

### ⚔️ Key Differences

| Feature      | Sync 🟡        | Async 🔵             |
|--------------|----------------|----------------------|
| Execution    | Sequential     | Non-blocking         |
| Blocking     | Yes            | No                   |
| Performance  | Slower (I/O)   | Faster (I/O)         |
| Complexity   | Low            | Medium               |

---

### 🎯 Interview Points

- JavaScript is single-threaded, async handled via Event Loop  
- Async ≠ parallel execution  
- setTimeout → Web APIs → Callback Queue → Event Loop  
- Async is best for API calls, DB ops, file handling  

---

- ## **Javascript is a language but Node.js is runtime(not a lang) that is used to run javascript(Week 2.1 15:31)**
- ## **WebRTC protocol is a protocol used for video communications (Week 2.1 22:12)**