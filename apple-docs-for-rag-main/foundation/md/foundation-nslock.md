

- Foundation
-  NSLock 

Class

# NSLock

An object that coordinates the operation of multiple threads of execution within the same application.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSLock
```

## Overview

An NSLock object can be used to mediate access to an application’s global data or to protect a critical section of code, allowing it to run atomically.

Warning

The NSLock class uses POSIX threads to implement its locking behavior. When sending an unlock message to an NSLock object, you must be sure that message is sent from the same thread that sent the initial lock message. Unlocking a lock from a different thread can result in undefined behavior.

You should not use this class to implement a recursive lock. Calling the `lock` method twice on the same thread will lock up your thread permanently. Use the NSRecursiveLock class to implement recursive locks instead.

Unlocking a lock that is not locked is considered a programmer error and should be fixed in your code. The NSLock class reports such errors by printing an error message to the console when they occur.

## Topics

### Acquiring a Lock

func lock(before: Date) -> Bool

Attempts to acquire a lock before a given time and returns a Boolean value indicating whether the attempt was successful.

func `try`() -> Bool

Attempts to acquire a lock and immediately returns a Boolean value that indicates whether the attempt was successful.

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

class NSRecursiveLock

A lock that may be acquired multiple times by the same thread without causing a deadlock.

class NSDistributedLock

A lock that multiple applications on multiple hosts can use to restrict access to some shared resource, such as a file.

class NSConditionLock

A lock that can be associated with specific, user-defined conditions.

class NSCondition

A condition variable whose semantics follow those used for POSIX-style conditions.

