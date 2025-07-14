

- Dispatch
- DispatchSourceProtocol
-  isCancelled 

Instance Property

# isCancelled

Returns a Boolean indicating whether the given dispatch source has been canceled.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isCancelled: Bool { get }
```

## See Also

### Canceling a Dispatch Source

func cancel()

Asynchronously cancels the dispatch source, preventing any further invocation of its event handler block.

func setCancelHandler(handler: DispatchWorkItem)

Sets the cancellation handler block for the dispatch source.

func setCancelHandler(qos: DispatchQoS, flags: DispatchWorkItemFlags, handler: Self.DispatchSourceHandler?)

Sets the cancellation handler block for the dispatch source with the specified quality-of-service class and work item options.

