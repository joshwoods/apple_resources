

- Foundation
- NSCondition
-  wait() 

Instance Method

# wait()

Blocks the current thread until the condition is signaled.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func wait()
```

## Discussion

You must lock the receiver prior to calling this method.

## See Also

### Related Documentation

Threading Programming Guide

func lock()

Attempts to acquire a lock, blocking a thread’s execution until the lock can be acquired.

**Required**

### Waiting for the Lock

func wait(until: Date) -> Bool

Blocks the current thread until the condition is signaled or the specified time limit is reached.

