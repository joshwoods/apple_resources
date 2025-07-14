

- Dispatch
- DispatchQueue
-  global(qos:) 

Type Method

# global(qos:)

Returns the global system queue with the specified quality-of-service class.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
class func global(qos: DispatchQoS.QoSClass = .default) -> DispatchQueue
```

## Parameters 

`qos`  

The quality-of-service level to associate with the queue. This value determines the priority at which the system schedules tasks for execution. For a list of possible values, see DispatchQoS.QoSClass.

## Discussion

This method returns a queue suitable for executing tasks with the specified quality-of-service level. Calls to the suspend(), resume(), and dispatch_set_context functions have no effect on the returned queues.

Tasks submitted to the returned queue are scheduled concurrently with respect to one another.

## See Also

### Creating a Dispatch Queue

class var main: DispatchQueue

The dispatch queue associated with the main thread of the current process.

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

