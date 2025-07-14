

- Foundation
- NSRecursiveLock
-  lock(before:) 

Instance Method

# lock(before:)

Attempts to acquire a lock before a given date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func lock(before limit: Date) -> Bool
```

## Parameters 

`limit`  

The time before which the lock should be acquired.

## Return Value

true if the lock is acquired before `limit`, otherwise false.

## Discussion

The thread is blocked until the receiver acquires the lock or `limit` is reached.

## See Also

### Related Documentation

Threading Programming Guide

### Acquiring a Lock

func `try`() -> Bool

Attempts to acquire a lock, and immediately returns a Boolean value that indicates whether the attempt was successful.

