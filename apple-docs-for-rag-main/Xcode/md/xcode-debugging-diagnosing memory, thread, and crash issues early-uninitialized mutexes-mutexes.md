

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Uninitialized mutexes 

Article

# Uninitialized mutexes

Detects when you use an uninitialized mutex.

## Overview

Use this check to detect when you call `pthread_mutex_lock(_:)` or `pthread_mutex_unlock(_:)` with an uninitialized `pthread_mutex_t` variable. Attempting to use an uninitialized mutex results in an error, and bypasses ordering conditions that exist on a locked mutex. Available in Xcode 8 and later.

### Use of uninitialized mutex in C

In the following example, the `pthread_mutex_lock(_:)` function executes with an uninitialized `pthread_mutex_t` variable:

```
static pthread_mutex_t mutex;
void performWork() {
    pthread_mutex_lock(&mutex); // Error: uninitialized mutex
    // ...
    pthread_mutex_unlock(&mutex);
}
```

#### Solution

Use the `pthread_once(_:_:)` function to initialize a mutex before you use it.

```
static pthread_once_t once = PTHREAD_ONCE_INIT;
static pthread_mutex_t mutex;
void init() {    
    pthread_mutex_init(&mutex, NULL);
}
void performWork() {
    pthread_once(&once, init); // Correct
    pthread_mutex_lock(&mutex);
    // ...
    pthread_mutex_unlock(&mutex);
}
```

## See Also

### Thread Sanitizer

Data races

Detects unsynchronized access to mutable state across multiple threads.

Swift access races

Detects unsynchronized access to mutable state across multiple threads in Swift.

Races on collections and other APIs

Detects when one thread accesses a mutable object while another thread is writing to it.

Thread leaks

Detects when you don’t close threads after use.

