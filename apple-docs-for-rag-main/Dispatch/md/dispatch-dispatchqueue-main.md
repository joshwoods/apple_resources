

- Dispatch
- DispatchQueue
-  main 

Type Property

# main

The dispatch queue associated with the main thread of the current process.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class var main: DispatchQueue { get }
```

## Discussion

The system automatically creates the main queue and associates it with your application’s main thread. Your app uses one (and only one) of the following three approaches to execute blocks submitted to the main queue:

- Calling dispatchMain()

- Starting your app with a call to UIApplicationMain(_:_:_:_:) (iOS) or NSApplicationMain(_:_:) (macOS)

- Using a CFRunLoop on the main thread

As with the global concurrent queues, calls to suspend(), resume(), dispatch_set_context, and the like have no effect when used on the queue in this property.

Important

If the main thread is unresponsive for too long, it can lead to a `0x8badf00d` exception with the main thread at `mach_msg_trap`. On iOS, this exception may be raised if the watchdog mechanism detects that your app failed to respond to certain user interface events in time. The iOS watchdog exists in order to keep the user interface responsive.

If your app has a long running task, such as making network call, run it on a global system queue, or on another background dispatch queue. Alternatively, use asynchronous versions of the call, if available.

## See Also

### Creating a Dispatch Queue

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

