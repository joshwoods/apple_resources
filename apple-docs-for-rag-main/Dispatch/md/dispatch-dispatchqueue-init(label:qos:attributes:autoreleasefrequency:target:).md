

- Dispatch
- DispatchQueue
-  init(label:qos:attributes:autoreleaseFrequency:target:) 

Initializer

# init(label:qos:attributes:autoreleaseFrequency:target:)

Creates a new dispatch queue to which you can submit blocks.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    label: String,
    qos: DispatchQoS = .unspecified,
    attributes: DispatchQueue.Attributes = [],
    autoreleaseFrequency: DispatchQueue.AutoreleaseFrequency = .inherit,
    target: DispatchQueue? = nil
)
```

## Parameters 

`label`  

A string label to attach to the queue to uniquely identify it in debugging tools such as Instruments, sample, stackshots, and crash reports. Because applications, libraries, and frameworks can all create their own dispatch queues, a reverse-DNS naming style (`com.example.myqueue`) is recommended. This parameter is optional and can be `NULL`.

`qos`  

The quality-of-service level to associate with the queue. This value determines the priority at which the system schedules tasks for execution. For a list of possible values, see DispatchQoS.QoSClass.

`attributes`  

The attributes to associate with the queue. Include the concurrent attribute to create a dispatch queue that executes tasks concurrently. If you omit that attribute, the dispatch queue executes tasks serially.

`autoreleaseFrequency`  

The frequency with which to autorelease objects created by the blocks that the queue schedules. For a list of possible values, see DispatchQueue.AutoreleaseFrequency.

`target`  

The target queue on which to execute blocks. Specify `DISPATCH_TARGET_QUEUE_DEFAULT` if you want the system to provide a queue that is appropriate for the current object.

## See Also

### Creating a Dispatch Queue

class var main: DispatchQueue

The dispatch queue associated with the main thread of the current process.

class func global(qos: DispatchQoS.QoSClass) -> DispatchQueue

Returns the global system queue with the specified quality-of-service class.

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

