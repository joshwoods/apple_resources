

- Dispatch
- DispatchSourceProtocol
-  setEventHandler(qos:flags:handler:) 

Instance Method

# setEventHandler(qos:flags:handler:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func setEventHandler(
    qos: DispatchQoS = .unspecified,
    flags: DispatchWorkItemFlags = [],
    handler: Self.DispatchSourceHandler?
)
```

## See Also

### Installing Event Handlers

func setEventHandler(handler: DispatchWorkItem)

Sets the event handler work item for the dispatch source.

func setRegistrationHandler(handler: DispatchWorkItem)

Sets the registration handler work item for the dispatch source.

func setRegistrationHandler(qos: DispatchQoS, flags: DispatchWorkItemFlags, handler: Self.DispatchSourceHandler?)

typealias DispatchSourceHandler

