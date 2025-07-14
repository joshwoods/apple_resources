

- Foundation
-  NSLocking 

Protocol

# NSLocking

The elementary methods adopted by classes that define lock objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSLocking
```

## Overview

A lock object is used to coordinate the actions of multiple threads of execution within a single application. By using a lock object, an application can protect critical sections of code from being executed simultaneously by separate threads, thus protecting shared data and other shared resources from corruption.

## Topics

### Working with Locks

func lock()

Attempts to acquire a lock, blocking a thread’s execution until the lock can be acquired.

**Required**

func unlock()

Relinquishes a previously acquired lock.

**Required**

### Instance Methods

func withLock&lt;R>(() throws -> R) rethrows -> R

## Relationships

### Conforming Types

- NSCondition
- NSConditionLock
- NSLock
- NSRecursiveLock

## See Also

### Threads and Locking

class Thread

A thread of execution.

class NSLock

An object that coordinates the operation of multiple threads of execution within the same application.

class NSRecursiveLock

A lock that may be acquired multiple times by the same thread without causing a deadlock.

class NSDistributedLock

A lock that multiple applications on multiple hosts can use to restrict access to some shared resource, such as a file.

class NSConditionLock

A lock that can be associated with specific, user-defined conditions.

class NSCondition

A condition variable whose semantics follow those used for POSIX-style conditions.

