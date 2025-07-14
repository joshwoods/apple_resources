

- Foundation
- Thread
-  start() 

Instance Method

# start()

Starts the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func start()
```

## Discussion

This method asynchronously spawns the new thread and invokes the receiver’s main() method on the new thread. The isExecuting property returns true once the thread starts executing, which may occur after the start() method returns.

If you initialized the receiver with a target and selector, the default main() method invokes that selector automatically.

If this thread is the first thread detached in the application, this method posts the NSWillBecomeMultiThreaded with object `nil` to the default notification center.

## See Also

### Related Documentation

convenience init(target: Any, selector: Selector, object: Any?)

Returns an `NSThread` object initialized with the given arguments.

init()

Returns an initialized `NSThread` object.

### Starting a Thread

class func detachNewThreadSelector(Selector, toTarget: Any, with: Any?)

Detaches a new thread and uses the specified selector as the thread entry point.

func main()

The main entry point routine for the thread.

