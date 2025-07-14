

- Dispatch
- DispatchSource
-  makeProcessSource(identifier:eventMask:queue:) 

Type Method

# makeProcessSource(identifier:eventMask:queue:)

Creates a new dispatch source object for monitoring the specified process.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func makeProcessSource(
    identifier: pid_t,
    eventMask: DispatchSource.ProcessEvent,
    queue: DispatchQueue? = nil
) -> any DispatchSourceProcess
```

## Parameters 

`identifier`  

The process identifier of the process you want to monitor.

`eventMask`  

The set of events you want to monitor. For a list of possible values, see DispatchSource.ProcessEvent.

`queue`  

The dispatch queue to use when executing the installed handlers.

## Return Value

A dispatch source object that conforms to the DispatchSourceProcess protocol.

## Discussion

After creating the dispatch source, use the methods of the DispatchSourceProtocol protocol to install the event handlers you need. The returned dispatch source is in the inactive state initially. When you are ready to begin processing events, call its activate() method.

## See Also

### Creating a Process Source

protocol DispatchSourceProcess

A dispatch source that monitors an external process for events.

struct ProcessEvent

Events related to a process.

