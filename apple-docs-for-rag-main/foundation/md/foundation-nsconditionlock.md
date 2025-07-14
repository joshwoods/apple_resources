

- Foundation
-  NSConditionLock 

Class

# NSConditionLock

A lock that can be associated with specific, user-defined conditions.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSConditionLock
```

## Overview

Using an NSConditionLock object, you can ensure that a thread can acquire a lock only if a certain condition is met. Once it has acquired the lock and executed the critical section of code, the thread can relinquish the lock and set the associated condition to something new. The conditions themselves are arbitrary: you define them as needed for your application.

## Topics

### Initializing an NSConditionLock Object

init(condition: Int)

Initializes a newly allocated `NSConditionLock` object and sets its condition.

### Accessing the Condition

var condition: Int

The condition associated with the receiver.

### Acquiring and Releasing a Lock

func lock(before: Date) -> Bool

Attempts to acquire a lock before a specified moment in time.

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

### Identifying the Condition Lock

var name: String?

The name associated with the receiver.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSLocking
- NSObjectProtocol
- Sendable

## See Also

### Threads and Locking

class Thread

A thread of execution.

protocol NSLocking

The elementary methods adopted by classes that define lock objects.

class NSLock

An object that coordinates the operation of multiple threads of execution within the same application.

class NSRecursiveLock

A lock that may be acquired multiple times by the same thread without causing a deadlock.

class NSDistributedLock

A lock that multiple applications on multiple hosts can use to restrict access to some shared resource, such as a file.

class NSCondition

A condition variable whose semantics follow those used for POSIX-style conditions.

