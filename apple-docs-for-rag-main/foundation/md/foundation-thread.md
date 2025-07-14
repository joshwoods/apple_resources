

- Foundation
-  Thread 

Class

# Thread

A thread of execution.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class Thread
```

## Overview

Use this class when you want to have an Objective-C method run in its own thread of execution. Threads are especially useful when you need to perform a lengthy task, but don’t want it to block the execution of the rest of the application. In particular, you can use threads to avoid blocking the main thread of the application, which handles user interface and event-related actions. Threads can also be used to divide a large job into several smaller jobs, which can lead to performance increases on multi-core computers.

The Thread class supports semantics similar to those of Operation for monitoring the runtime condition of a thread. You can use these semantics to cancel the execution of a thread or determine if the thread is still executing or has finished its task. Canceling a thread requires support from your thread code; see the description for cancel() for more information.

### Subclassing Notes

You can subclass Thread and override the main() method to implement your thread’s main entry point. If you override main(), you do not need to invoke the inherited behavior by calling `super`.

## Topics

### Initializing an NSThread Object

init()

Returns an initialized `NSThread` object.

convenience init(target: Any, selector: Selector, object: Any?)

Returns an `NSThread` object initialized with the given arguments.

### Starting a Thread

class func detachNewThreadSelector(Selector, toTarget: Any, with: Any?)

Detaches a new thread and uses the specified selector as the thread entry point.

func start()

Starts the receiver.

func main()

The main entry point routine for the thread.

### Stopping a Thread

class func sleep(until: Date)

Blocks the current thread until the time specified.

class func sleep(forTimeInterval: TimeInterval)

Sleeps the thread for a given time interval.

class func exit()

Terminates the current thread.

func cancel()

Changes the cancelled state of the receiver to indicate that it should exit.

### Determining the Thread’s Execution State

var isExecuting: Bool

A Boolean value that indicates whether the receiver is executing.

var isFinished: Bool

A Boolean value that indicates whether the receiver has finished execution.

var isCancelled: Bool

A Boolean value that indicates whether the receiver is cancelled.

### Working with the Main Thread

class var isMainThread: Bool

Returns a Boolean value that indicates whether the current thread is the main thread.

var isMainThread: Bool

A Boolean value that indicates whether the receiver is the main thread.

class var main: Thread

Returns the `NSThread` object representing the main thread.

### Querying the Environment

class func isMultiThreaded() -> Bool

Returns whether the application is multithreaded.

class var current: Thread

Returns the thread object representing the current thread of execution.

class var callStackReturnAddresses: [NSNumber]

Returns an array containing the call stack return addresses.

class var callStackSymbols: [String]

Returns an array containing the call stack symbols.

### Working with Thread Properties

var threadDictionary: NSMutableDictionary

The thread object’s dictionary.

let NSAssertionHandlerKey: String

var name: String?

The name of the receiver.

var stackSize: Int

The stack size of the receiver, in bytes.

### Prioritizing Thread Work

var qualityOfService: QualityOfService

enum QualityOfService

Constants that indicate the nature and importance of work to the system.

class func threadPriority() -> Double

Returns the current thread’s priority.

var threadPriority: Double

The receiver’s priority

class func setThreadPriority(Double) -> Bool

Sets the current thread’s priority.

### Notifications

static let NSDidBecomeSingleThreaded: NSNotification.Name

Not implemented.

static let NSThreadWillExit: NSNotification.Name

An `NSThread` object posts this notification when it receives the exit() message, before the thread exits. Observer methods invoked to receive this notification execute in the exiting thread, before it exits.

static let NSWillBecomeMultiThreaded: NSNotification.Name

Posted when the first thread is detached from the current thread. The `NSThread` class posts this notification at most once—the first time a thread is detached using detachNewThreadSelector(_:toTarget:with:) or the start() method. Subsequent invocations of those methods do not post this notification. Observers of this notification have their notification method invoked in the main thread, not the new thread. The observer notification methods always execute before the new thread begins executing.

### Initializers

convenience init(block: () -> Void)

### Type Methods

class func detachNewThread(() -> Void)

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

## See Also

### Threads and Locking

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

