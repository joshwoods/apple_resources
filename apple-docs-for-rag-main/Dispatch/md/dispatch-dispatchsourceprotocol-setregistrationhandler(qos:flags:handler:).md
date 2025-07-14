

- Dispatch
- DispatchSourceProtocol
-  setRegistrationHandler(qos:flags:handler:) 

Instance Method

# setRegistrationHandler(qos:flags:handler:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func setRegistrationHandler(
    qos: DispatchQoS = .unspecified,
    flags: DispatchWorkItemFlags = [],
    handler: Self.DispatchSourceHandler?
)
```

## See Also

### Installing Event Handlers

func setEventHandler(handler: DispatchWorkItem)

Sets the event handler work item for the dispatch source.

func setEventHandler(qos: DispatchQoS, flags: DispatchWorkItemFlags, handler: Self.DispatchSourceHandler?)

func setRegistrationHandler(handler: DispatchWorkItem)

Sets the registration handler work item for the dispatch source.

typealias DispatchSourceHandler

