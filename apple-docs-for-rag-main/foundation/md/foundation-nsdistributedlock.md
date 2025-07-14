

- Foundation
-  NSDistributedLock 

Class

# NSDistributedLock

A lock that multiple applications on multiple hosts can use to restrict access to some shared resource, such as a file.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSDistributedLock
```

## Overview

The lock is implemented by an entry (such as a file or directory) in the file system. For multiple applications to use an NSDistributedLock object to coordinate their activities, the lock must be writable on a file system accessible to all hosts on which the applications might be running.

Use the try() method to attempt to acquire a lock. You should generally use the unlock() method to release the lock rather than break().

NSDistributedLock doesn’t conform to the NSLocking protocol, nor does it have a `lock` method. The protocol’s lock() method is intended to block the execution of the thread until successful. For an NSDistributedLock object, this could mean polling the file system at some predetermined rate. A better solution is to provide the try() method and let you determine the polling frequency that makes sense for your application.

## Topics

### Creating an NSDistributedLock

init?(path: String)

Initializes an `NSDistributedLock` object to use as the lock the file-system entry specified by a given path.

### Acquiring a Lock

func `try`() -> Bool

Attempts to acquire the receiver and immediately returns a Boolean value that indicates whether the attempt was successful.

### Relinquishing a Lock

func `break`()

Forces the lock to be relinquished.

func unlock()

Relinquishes the receiver.

### Getting Lock Information

var lockDate: Date

Returns the time the receiver was acquired by any of the `NSDistributedLock` objects using the same path.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
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

class NSConditionLock

A lock that can be associated with specific, user-defined conditions.

class NSCondition

A condition variable whose semantics follow those used for POSIX-style conditions.

