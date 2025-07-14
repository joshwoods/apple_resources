

- Dispatch
-  DispatchQueue 

Class

# DispatchQueue

An object that manages the execution of tasks serially or concurrently on your app’s main thread or on a background thread.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class DispatchQueue
```

## Overview

Dispatch queues are FIFO queues to which your application can submit tasks in the form of block objects. Dispatch queues execute tasks either serially or concurrently. Work submitted to dispatch queues executes on a pool of threads managed by the system. Except for the dispatch queue representing your app’s main thread, the system makes no guarantees about which thread it uses to execute a task.

You schedule work items synchronously or asynchronously. When you schedule a work item synchronously, your code waits until that item finishes execution. When you schedule a work item asynchronously, your code continues executing while the work item runs elsewhere.

Important

Attempting to synchronously execute a work item on the main queue results in deadlock.

### Avoiding Excessive Thread Creation

When designing tasks for concurrent execution, do not call methods that block the current thread of execution. When a task scheduled by a concurrent dispatch queue blocks a thread, the system creates additional threads to run other queued concurrent tasks. If too many tasks block, the system may run out of threads for your app.

Another way that apps consume too many threads is by creating too many private concurrent dispatch queues. Because each dispatch queue consumes thread resources, creating additional concurrent dispatch queues exacerbates the thread consumption problem. Instead of creating private concurrent queues, submit tasks to one of the global concurrent dispatch queues. For serial tasks, set the target of your serial queue to one of the global concurrent queues. That way, you can maintain the serialized behavior of the queue while minimizing the number of separate queues creating threads.

## Topics

### Creating a Dispatch Queue

class var main: DispatchQueue

The dispatch queue associated with the main thread of the current process.

class func global(qos: DispatchQoS.QoSClass) -> DispatchQueue

Returns the global system queue with the specified quality-of-service class.

convenience init(label: String, qos: DispatchQoS, attributes: DispatchQueue.Attributes, autoreleaseFrequency: DispatchQueue.AutoreleaseFrequency, target: DispatchQueue?)

Creates a new dispatch queue to which you can submit blocks.

enum QoSClass

Quality-of-service classes that specify the priorities for executing tasks.

struct Attributes

Attributes that define the behavior of a dispatch queue.

enum AutoreleaseFrequency

Constants indicating the frequency with which a dispatch queue autoreleases objects.

class OS_dispatch_queue_main

A system-provided dispatch queue that schedules tasks for serial execution on the app’s main thread.

class OS_dispatch_queue_global

A system-provided dispatch queue that schedules tasks for concurrent execution.

class DispatchSerialQueue

A custom dispatch queue that schedules tasks for serial execution on an arbitrary thread.

class DispatchConcurrentQueue

A custom dispatch queue that schedules tasks for concurrent execution.

typealias dispatch_queue_main_t

A dispatch queue that is bound to the app’s main thread and executes tasks serially on that thread.

typealias dispatch_queue_global_t

A dispatch queue that executes tasks concurrently using threads from the global thread pool.

typealias dispatch_queue_serial_t

A dispatch queue that executes tasks serially in first-in, first-out (FIFO) order.

typealias dispatch_queue_concurrent_t

A dispatch queue that executes tasks concurrently and in any order, respecting any barriers that may be in place.

### Executing Tasks Asynchronously

func async(execute: DispatchWorkItem)

Schedules a work item for immediate execution, and returns immediately.

func asyncAfter(deadline: DispatchTime, execute: DispatchWorkItem)

Schedules a work item for execution at the specified time, and returns immediately.

func asyncAfter(deadline: DispatchTime, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

Schedules a block for execution using the specified attributes, and returns immediately.

func asyncAfter(wallDeadline: DispatchWallTime, execute: DispatchWorkItem)

Schedules a work item for execution after the specified time, and returns immediately.

func asyncAfter(wallDeadline: DispatchWallTime, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

Schedules a block for execution using the specified attributes, and returns immediately.

### Executing Tasks Synchronously

func sync(execute: DispatchWorkItem)

Submits a work item for execution on the current queue and returns after that block finishes executing.

func sync(execute: () -> Void)

Submits a block object for execution and returns after that block finishes executing.

func sync&lt;T>(execute: () throws -> T) rethrows -> T

Submits a work item for execution and returns the results from that item after it finishes executing.

func sync&lt;T>(flags: DispatchWorkItemFlags, execute: () throws -> T) rethrows -> T

Submits a work item for execution using the specified attributes and returns the results from that item after it finishes executing.

func asyncAndWait(execute: () -> Void)

Submits a work item for execution and returns only after it finishes executing.

### Executing a Task in Parallel

class func concurrentPerform(iterations: Int, execute: (Int) -> Void)

Submits a single block to the dispatch queue and causes the block to be executed the specified number of times.

### Dispatching Work to Groups

func async(group: DispatchGroup, execute: DispatchWorkItem)

Schedules a work item asynchronously for execution and associates it with the specified dispatch group.

func async(group: DispatchGroup?, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

Schedules a block asynchronously for execution and optionally associates it with a dispatch group.

### Managing Queue Attributes

var label: String

The label you assigned to the dispatch queue at creation time.

var qos: DispatchQoS

The quality-of-service level assgined to the queue.

func setTarget(queue: dispatch_queue_t?)

Specifies the dispatch queue on which to perform work associated with the current object.

### Getting and Setting Contextual Data

func setSpecific&lt;T>(key: DispatchSpecificKey&lt;T>, value: T?)

Sets the key/value data for the specified dispatch queue.

func getSpecific&lt;T>(key: DispatchSpecificKey&lt;T>) -> T?

Returns the value for the key associated with this dispatch queue.

class func getSpecific&lt;T>(key: DispatchSpecificKey&lt;T>) -> T?

Returns the value for the key associated with the current execution context.

class DispatchSpecificKey

A key associated with a specific contextual value on a dispatch queue.

### Managing the Main Dispatch Queue

func dispatchMain() -> Never

Executes blocks submitted to the main queue.

### Scheduling Combine Publishers

struct SchedulerTimeType

The scheduler time type used by the dispatch queue.

struct SchedulerOptions

A set of options that affect the operation of the dispatch queue scheduler.

### Deprecated

class func global(priority: DispatchQueue.GlobalQueuePriority) -> DispatchQueue

enum GlobalQueuePriority

Legacy constants for queue priorities.

### Instance Methods

func asyncAfterUnsafe(deadline: DispatchTime, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

func asyncAfterUnsafe(wallDeadline: DispatchWallTime, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

func asyncAndWait&lt;T>(execute: () throws -> T) rethrows -> T

func asyncAndWait(execute: DispatchWorkItem)

func asyncAndWait&lt;T>(flags: DispatchWorkItemFlags, execute: () throws -> T) rethrows -> T

func asyncUnsafe(group: DispatchGroup?, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

### Default Implementations

Scheduler Implementations

## Relationships

### Inherits From

- DispatchObject

### Inherited By

- DispatchConcurrentQueue
- DispatchSerialQueue
- DispatchWorkloop
- OS_dispatch_queue_global

### Conforms To

- CVarArg
- Copyable
- Equatable
- Executor
- Hashable
- NSObjectProtocol
- Scheduler
- Sendable
- TaskExecutor

## See Also

### Queues and Tasks

class DispatchWorkItem

The work you want to perform, encapsulated in a way that lets you attach a completion handle or execution dependencies.

class DispatchGroup

A group of tasks that you monitor as a single unit.

Dispatch Queue

An object that manages the execution of tasks serially or concurrently on your app’s main thread or on a background thread.

Dispatch Work Item

The work you want to perform, encapsulated in a way that lets you attach a completion handle or execution dependencies.

Dispatch Group

A group of tasks that you monitor as a single unit.

Workloop

A dispatch object that prioritizes the execution of tasks based on their quality-of-service (QoS) level.

