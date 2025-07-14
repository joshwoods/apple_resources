

- Dispatch
- DispatchSourceProtocol
-  cancel() 

Instance Method

# cancel()

Asynchronously cancels the dispatch source, preventing any further invocation of its event handler block.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func cancel()
```

## Discussion

Cancellation prevents any further invocation of the event handler block for the dispatch source, but does not interrupt any work that is already in progress. If a cancellation handler was set before cancellation, it is sub mitted to the target queue once any in-progress event handler work is finished. Once the cancellation handler is submitted, it is safe to close the source’s handle (file descriptor or mach port). It is invalid to close a file descriptor or deallocate a mach port that is currently being tracked by a dispatch source object before the cancellation handler is invoked.

## See Also

### Canceling a Dispatch Source

var isCancelled: Bool

Returns a Boolean indicating whether the given dispatch source has been canceled.

func setCancelHandler(handler: DispatchWorkItem)

Sets the cancellation handler block for the dispatch source.

func setCancelHandler(qos: DispatchQoS, flags: DispatchWorkItemFlags, handler: Self.DispatchSourceHandler?)

Sets the cancellation handler block for the dispatch source with the specified quality-of-service class and work item options.

