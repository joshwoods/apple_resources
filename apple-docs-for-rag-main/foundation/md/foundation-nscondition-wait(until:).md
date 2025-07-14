

- Foundation
- NSCondition
-  wait(until:) 

Instance Method

# wait(until:)

Blocks the current thread until the condition is signaled or the specified time limit is reached.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func wait(until limit: Date) -> Bool
```

## Parameters 

`limit`  

The time at which to wake up the thread if the condition has not been signaled.

## Return Value

true if the condition was signaled; otherwise, false if the time limit was reached.

## Discussion

You must lock the receiver prior to calling this method.

## See Also

### Related Documentation

func lock()

Attempts to acquire a lock, blocking a thread’s execution until the lock can be acquired.

**Required**

### Waiting for the Lock

func wait()

Blocks the current thread until the condition is signaled.

