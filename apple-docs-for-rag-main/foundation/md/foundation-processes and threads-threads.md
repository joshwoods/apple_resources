

- Foundation
-  Processes and Threads 

API Collection

# Processes and Threads

Manage your app’s interaction with the host operating system and other processes, and implement low-level concurrency features.

## Topics

### Run Loop Scheduling

class RunLoop

The programmatic interface to objects that manage input sources.

class Timer

A timer that fires after a certain time interval has elapsed, sending a specified message to a target object.

### Process Info

class ProcessInfo

A collection of information about the current process.

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

class NSCondition

A condition variable whose semantics follow those used for POSIX-style conditions.

### Operations

class OperationQueue

A queue that regulates the execution of operations.

class Operation

An abstract class that represents the code and data associated with a single task.

class BlockOperation

An operation that manages the concurrent execution of one or more blocks.

### Scripts and External Tasks

class Process

An object that represents a subprocess of the current process.

class NSUserScriptTask

An object that executes scripts.

class NSUserAppleScriptTask

An object that executes AppleScript scripts.

class NSUserAutomatorTask

An object that executes Automator workflows.

class NSUserUnixTask

An object that executes unix applications.

## See Also

### Low-Level Utilities

XPC

Manage secure interprocess communication.

Object Runtime

Get low-level support for basic Objective-C features, Cocoa design patterns, and Swift integration.

Streams, Sockets, and Ports

Use low-level Unix features to manage input and output among files, processes, and the network.

