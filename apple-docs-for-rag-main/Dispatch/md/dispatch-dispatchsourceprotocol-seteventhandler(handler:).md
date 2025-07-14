

- Dispatch
- DispatchSourceProtocol
-  setEventHandler(handler:) 

Instance Method

# setEventHandler(handler:)

Sets the event handler work item for the dispatch source.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func setEventHandler(handler: DispatchWorkItem)
```

## Parameters 

`handler`  

The event handler block to submit to the source’s target queue.

## Discussion

The event handler (if specified) is submitted to the source’s target queue in response to the arrival of an event.

## See Also

### Installing Event Handlers

func setEventHandler(qos: DispatchQoS, flags: DispatchWorkItemFlags, handler: Self.DispatchSourceHandler?)

func setRegistrationHandler(handler: DispatchWorkItem)

Sets the registration handler work item for the dispatch source.

func setRegistrationHandler(qos: DispatchQoS, flags: DispatchWorkItemFlags, handler: Self.DispatchSourceHandler?)

typealias DispatchSourceHandler

