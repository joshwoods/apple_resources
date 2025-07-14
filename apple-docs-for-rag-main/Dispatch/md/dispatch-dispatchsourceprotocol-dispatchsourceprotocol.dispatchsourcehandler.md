

- Dispatch
- DispatchSourceProtocol
-  DispatchSourceProtocol.DispatchSourceHandler 

Type Alias

# DispatchSourceProtocol.DispatchSourceHandler

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias DispatchSourceHandler = () -> Void
```

## See Also

### Installing Event Handlers

func setEventHandler(handler: DispatchWorkItem)

Sets the event handler work item for the dispatch source.

func setEventHandler(qos: DispatchQoS, flags: DispatchWorkItemFlags, handler: Self.DispatchSourceHandler?)

func setRegistrationHandler(handler: DispatchWorkItem)

Sets the registration handler work item for the dispatch source.

func setRegistrationHandler(qos: DispatchQoS, flags: DispatchWorkItemFlags, handler: Self.DispatchSourceHandler?)

