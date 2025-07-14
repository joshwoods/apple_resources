

- Foundation
- Thread
-  detachNewThreadSelector(\_:toTarget:with:) 

Type Method

# detachNewThreadSelector(\_:toTarget:with:)

Detaches a new thread and uses the specified selector as the thread entry point.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func detachNewThreadSelector(
    _ selector: Selector,
    toTarget target: Any,
    with argument: Any?
)
```

## Parameters 

`selector`  

The selector for the message to send to the target. This selector must take only one argument and must not have a return value.

`target`  

The object that will receive the message `aSelector` on the new thread.

`argument`  

The single argument passed to the target. May be `nil`.

## Discussion

The objects `aTarget` and `anArgument` are retained during the execution of the detached thread, then released. The detached thread is exited (using the exit() class method) as soon as `aTarget` has completed executing the `aSelector` method.

If this thread is the first thread detached in the application, this method posts the NSWillBecomeMultiThreaded with object `nil` to the default notification center.

## See Also

### Related Documentation

class func isMultiThreaded() -> Bool

Returns whether the application is multithreaded.

class var current: Thread

Returns the thread object representing the current thread of execution.

### Starting a Thread

func start()

Starts the receiver.

func main()

The main entry point routine for the thread.

