

- Foundation
-  NSCondition 

Class

# NSCondition

A condition variable whose semantics follow those used for POSIX-style conditions.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSCondition
```

## Overview

A condition object acts as both a lock and a checkpoint in a given thread. The lock protects your code while it tests the condition and performs the task triggered by the condition. The checkpoint behavior requires that the condition be true before the thread proceeds with its task. While the condition is not true, the thread blocks. It remains blocked until another thread signals the condition object.

The semantics for using an NSCondition object are as follows:

1.  Lock the condition object.

2.  Test a boolean predicate. (This predicate is a boolean flag or other variable in your code that indicates whether it is safe to perform the task protected by the condition.)

3.  If the boolean predicate is false, call the condition object’s wait() or wait(until:) method to block the thread. Upon returning from these methods, go to step 2 to retest your boolean predicate. (Continue waiting and retesting the predicate until it is true.)

4.  If the boolean predicate is true, perform the task.

5.  Optionally update any predicates (or signal any conditions) affected by your task.

6.  When your task is done, unlock the condition object.

The pseudocode for performing the preceding steps would therefore look something like the following:

```
lock the condition
while (!(boolean_predicate)) {
    wait on condition
}
do protected work
(optionally, signal or broadcast the condition again or change a predicate value)
unlock the condition
```

Whenever you use a condition object, the first step is to lock the condition. Locking the condition ensures that your predicate and task code are protected from interference by other threads using the same condition. Once you have completed your task, you can set other predicates or signal other conditions based on the needs of your code. You should always set predicates and signal conditions while holding the condition object’s lock.

When a thread waits on a condition, the condition object unlocks its lock and blocks the thread. When the condition is signaled, the system wakes up the thread. The condition object then reacquires its lock before returning from the wait() or wait(until:) method. Thus, from the point of view of the thread, it is as if it always held the lock.

A boolean predicate is an important part of the semantics of using conditions because of the way signaling works. Signaling a condition does not guarantee that the condition itself is true. There are timing issues involved in signaling that may cause false signals to appear. Using a predicate ensures that these spurious signals do not cause you to perform work before it is safe to do so. The predicate itself is simply a flag or other variable in your code that you test in order to acquire a Boolean result.

For more information on how to use conditions, see Using POSIX Thread Locks in Threading Programming Guide.

## Topics

### Waiting for the Lock

func wait()

Blocks the current thread until the condition is signaled.

func wait(until: Date) -> Bool

Blocks the current thread until the condition is signaled or the specified time limit is reached.

### Signaling Waiting Threads

func signal()

Signals the condition, waking up one thread waiting on it.

func broadcast()

Signals the condition, waking up all threads waiting on it.

### Identifying the Condition

var name: String?

The name of the condition.

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

class NSConditionLock

A lock that can be associated with specific, user-defined conditions.

