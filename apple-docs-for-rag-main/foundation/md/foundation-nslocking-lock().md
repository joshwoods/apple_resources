

- Foundation
- NSLocking
-  lock() 

Instance Method

# lock()

Attempts to acquire a lock, blocking a thread’s execution until the lock can be acquired.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func lock()
```

**Required**

## Discussion

An application protects a critical section of code by requiring a thread to acquire a lock before executing the code. Once the critical section is completed, the thread relinquishes the lock by invoking unlock().

## See Also

### Related Documentation

Threading Programming Guide

### Working with Locks

func unlock()

Relinquishes a previously acquired lock.

**Required**

