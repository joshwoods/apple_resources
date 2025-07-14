

- Foundation
- NSConditionLock
-  lock(whenCondition:before:) 

Instance Method

# lock(whenCondition:before:)

Attempts to acquire a lock before a specified moment in time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func lock(
    whenCondition condition: Int,
    before limit: Date
) -> Bool
```

## Parameters 

`condition`  

The condition to match on.

`limit`  

The date by which the lock must be acquired or the attempt will time out.

## Return Value

true if the lock is acquired within the time limit, false otherwise.

## Discussion

The receiver’s condition must be equal to `condition` before the locking operation will succeed. This method blocks the thread’s execution until the lock can be acquired or `limit` is reached.

## See Also

### Acquiring and Releasing a Lock

func lock(before: Date) -> Bool

Attempts to acquire a lock before a specified moment in time.

func lock(whenCondition: Int)

Attempts to acquire a lock.

func `try`() -> Bool

Attempts to acquire a lock without regard to the receiver’s condition.

func tryLock(whenCondition: Int) -> Bool

Attempts to acquire a lock if the receiver’s condition is equal to the specified condition.

func unlock(withCondition: Int)

Relinquishes the lock and sets the receiver’s condition.

