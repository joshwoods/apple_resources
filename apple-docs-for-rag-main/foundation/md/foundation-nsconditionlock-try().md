

- Foundation
- NSConditionLock
-  try() 

Instance Method

# try()

Attempts to acquire a lock without regard to the receiver’s condition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func `try`() -> Bool
```

## Return Value

true if the lock could be acquired, false otherwise.

## Discussion

This method returns immediately.

## See Also

### Acquiring and Releasing a Lock

func lock(before: Date) -> Bool

Attempts to acquire a lock before a specified moment in time.

func lock(whenCondition: Int)

Attempts to acquire a lock.

func lock(whenCondition: Int, before: Date) -> Bool

Attempts to acquire a lock before a specified moment in time.

func tryLock(whenCondition: Int) -> Bool

Attempts to acquire a lock if the receiver’s condition is equal to the specified condition.

func unlock(withCondition: Int)

Relinquishes the lock and sets the receiver’s condition.

