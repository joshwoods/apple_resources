

- Foundation
-  NSRecursiveLock 

Class

# NSRecursiveLock

A lock that may be acquired multiple times by the same thread without causing a deadlock.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSRecursiveLock
```

## Overview

NSRecursiveLock defines a lock that may be acquired multiple times by the same thread without causing a deadlock, a situation where a thread is permanently blocked waiting for itself to relinquish a lock. While the locking thread has one or more locks, all other threads are prevented from accessing the code protected by the lock.

## Topics

### Acquiring a Lock

func lock(before: Date) -> Bool

Attempts to acquire a lock before a given date.

func `try`() -> Bool

Attempts to acquire a lock, and immediately returns a Boolean value that indicates whether the attempt was successful.

### Naming the Lock

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

class NSDistributedLock

A lock that multiple applications on multiple hosts can use to restrict access to some shared resource, such as a file.

class NSConditionLock

A lock that can be associated with specific, user-defined conditions.

class NSCondition

A condition variable whose semantics follow those used for POSIX-style conditions.

