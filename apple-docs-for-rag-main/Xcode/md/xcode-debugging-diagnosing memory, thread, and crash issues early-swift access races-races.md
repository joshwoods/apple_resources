

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Swift access races 

Article

# Swift access races

Detects unsynchronized access to mutable state across multiple threads in Swift.

## Overview

Use this check to detect when multiple threads call a mutating method on a structure, or when they pass a reference to a shared variable without synchronization, which can result in unpredictable behavior. Available in Xcode 9 and later.

### Access race with mutating structure methods

In the following example, the `producer()` function adds messages to a global array, and the `consumer()` function removes messages from the array and prints them. Because `producer()` executes on one thread and `consumer()` executes on another, and both call mutating methods on the array, there is an access race on `messages`.

```
var messages: [String] = []
// Executed on Thread #1
func producer() {
    messages.append("A message");
}
// Executed on Thread #2
func consumer() {
    repeat {
        let message = messages.remove(at: 0)
        print("\(message)")
    } while !messages.isEmpty
}
```

#### Solution

Use Dispatch APIs to coordinate access to `messages` across multiple threads.

### Access race with in-out parameters

In the following example, the `writeNumbers()` function writes numbers to a global string. The `writeLetters()` function writes letters to the same string. Because the two functions execute on different threads and both access `log` by reference using `inout,` there is an access race on `log`.

```
var log: String = ""
// Executed on Thread #1
func writeNumbers() {
    print(1, 2, 3, separator: ",", to: &log)
}
// Executed on Thread #2
func writeLetters() {
    print("a", "b", "c", separator:",", to: &log)
}
```

#### Solution

Use Dispatch APIs to coordinate access to `log` across multiple threads.

## See Also

### Thread Sanitizer

Data races

Detects unsynchronized access to mutable state across multiple threads.

Races on collections and other APIs

Detects when one thread accesses a mutable object while another thread is writing to it.

Uninitialized mutexes

Detects when you use an uninitialized mutex.

Thread leaks

Detects when you don’t close threads after use.

