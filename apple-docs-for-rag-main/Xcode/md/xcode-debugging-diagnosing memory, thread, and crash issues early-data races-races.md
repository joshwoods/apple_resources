

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Data races 

Article

# Data races

Detects unsynchronized access to mutable state across multiple threads.

## Overview

Use this check to detect when multiple threads access the same memory without synchronization, and at least one access is a write. Available in Xcode 8 and later.

### Data race with producer and consumer functions

In the following example, the `producer()` function sets the global variable `message`, and the `consumer()` function waits for a flag to set before printing the message. Because `producer()` executes on one thread and `consumer()` executes on another thread, their execution can be concurrent, creating a data race.

```
var message: String? = nil
var messageIsAvailable: Bool = false
// Executed on Thread #1
func producer() {
    message = "hello!"
    messageIsAvailable = true
}
// Executed on Thread #2
func consumer() {
    repeat {
        usleep(1000)
    } while !messageIsAvailable
    print(message)
}
```

#### Solution

Use Dispatch APIs to coordinate access to `message` across multiple threads.

## See Also

### Thread Sanitizer

Swift access races

Detects unsynchronized access to mutable state across multiple threads in Swift.

Races on collections and other APIs

Detects when one thread accesses a mutable object while another thread is writing to it.

Uninitialized mutexes

Detects when you use an uninitialized mutex.

Thread leaks

Detects when you don’t close threads after use.

