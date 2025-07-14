

- Foundation
- NSConditionLock
-  lock(before:) 

Instance Method

# lock(before:)

Attempts to acquire a lock before a specified moment in time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func lock(before limit: Date) -> Bool
```

## Parameters 

`limit`  

The date by which the lock must be acquired or the attempt will time out.

## Return Value

true if the lock is acquired within the time limit, false otherwise.

## Discussion

The condition associated with the receiver isn’t taken into account in this operation. This method blocks the thread’s execution until the receiver acquires the lock or `limit` is reached.

## See Also

### Acquiring and Releasing a Lock

func lock(whenCondition: Int)

Attempts to acquire a lock.

func lock(whenCondition: Int, before: Date) -> Bool

Attempts to acquire a lock before a specified moment in time.

func `try`() -> Bool

Attempts to acquire a lock without regard to the receiver’s condition.

func tryLock(whenCondition: Int) -> Bool

Attempts to acquire a lock if the receiver’s condition is equal to the specified condition.

func unlock(withCondition: Int)

Relinquishes the lock and sets the receiver’s condition.

