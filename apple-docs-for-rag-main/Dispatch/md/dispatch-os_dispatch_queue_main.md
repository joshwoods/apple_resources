

- Dispatch
-  OS_dispatch_queue_main 

Class

# OS_dispatch_queue_main

A system-provided dispatch queue that schedules tasks for serial execution on the app’s main thread.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class OS_dispatch_queue_main
```

## Overview

You do not create objects of this type directly. You receive a queue of the appropriate type when you create a new DispatchQueue object.

## Relationships

### Inherits From

- DispatchSerialQueue

### Conforms To

- CVarArg
- Equatable
- Executor
- Hashable
- NSObjectProtocol
- Scheduler
- Sendable
- SerialExecutor
- TaskExecutor

## See Also

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

