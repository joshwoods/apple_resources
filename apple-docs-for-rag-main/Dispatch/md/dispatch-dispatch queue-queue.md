

- Dispatch
-  Dispatch Queue 

API Collection

# Dispatch Queue

An object that manages the execution of tasks serially or concurrently on your app’s main thread or on a background thread.

## Overview

Dispatch queues are FIFO queues to which your application can submit tasks in the form of block objects. Dispatch queues execute tasks either serially or concurrently. Work submitted to dispatch queues executes on a pool of threads managed by the system. Except for the dispatch queue representing your app’s main thread, the system makes no guarantees about which thread it uses to execute a task.

You schedule work items synchronously or asynchronously. When you schedule a work item synchronously, your code waits until that item finishes execution. When you schedule a work item asynchronously, your code continues executing while the work item runs elsewhere.

Important

Attempting to synchronously execute a work item on the main queue results in deadlock.

Dispatch queues provide minimal support for autoreleased objects by default. System APIs may return autoreleased objects to your code. For example, NSError objects are often autoreleased. If you see memory pressure increase because of autoreleased objects created in your blocks, consider adding autorelease pools to those blocks to relieve the pressure. You can also configure the default autorelease behavior of any custom dispatch queues using the dispatch_queue_attr_make_with_autorelease_frequency function at creation time.

### Avoiding Excessive Thread Creation

When designing tasks for concurrent execution, do not call methods that block the current thread of execution. When a task scheduled by a concurrent dispatch queue blocks a thread, the system creates additional threads to run other queued concurrent tasks. If too many tasks block, the system may run out of threads for your app.

Another way that apps consume too many threads is by creating too many private concurrent dispatch queues. Because each dispatch queue consumes thread resources, creating additional concurrent dispatch queues exacerbates the thread consumption problem. Instead of creating private concurrent queues, submit tasks to one of the global concurrent dispatch queues. For serial tasks, set the target of your serial queue to one of the global concurrent queues. That way, you can maintain the serialized behavior of the queue while minimizing the number of separate queues creating threads.

## Topics

### Creating a Dispatch Queue

typealias dispatch_queue_t

A lightweight object to which your application submits blocks for subsequent execution.

typealias dispatch_queue_main_t

A dispatch queue that is bound to the app’s main thread and executes tasks serially on that thread.

typealias dispatch_queue_global_t

A dispatch queue that executes tasks concurrently using threads from the global thread pool.

typealias dispatch_queue_serial_t

A dispatch queue that executes tasks serially in first-in, first-out (FIFO) order.

typealias dispatch_queue_concurrent_t

A dispatch queue that executes tasks concurrently and in any order, respecting any barriers that may be in place.

### Configuring Queue Execution Parameters

typealias dispatch_queue_attr_t

Attributes describing the behaviors of a dispatch queue.

### Executing Tasks Synchronously

func sync(execute: () -> Void)

Submits a block object for execution and returns after that block finishes executing.

func asyncAndWait(execute: () -> Void)

Submits a work item for execution and returns only after it finishes executing.

### Managing Queue Attributes

func setTarget(queue: dispatch_queue_t?)

Specifies the dispatch queue on which to perform work associated with the current object.

### Managing the Main Dispatch Queue

func dispatchMain() -> Never

Executes blocks submitted to the main queue.

## See Also

### Queues and Tasks

class DispatchQueue

An object that manages the execution of tasks serially or concurrently on your app’s main thread or on a background thread.

class DispatchWorkItem

The work you want to perform, encapsulated in a way that lets you attach a completion handle or execution dependencies.

class DispatchGroup

A group of tasks that you monitor as a single unit.

Dispatch Work Item

The work you want to perform, encapsulated in a way that lets you attach a completion handle or execution dependencies.

Dispatch Group

A group of tasks that you monitor as a single unit.

Workloop

A dispatch object that prioritizes the execution of tasks based on their quality-of-service (QoS) level.

