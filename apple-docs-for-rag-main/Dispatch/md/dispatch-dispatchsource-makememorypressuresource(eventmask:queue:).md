

- Dispatch
- DispatchSource
-  makeMemoryPressureSource(eventMask:queue:) 

Type Method

# makeMemoryPressureSource(eventMask:queue:)

Creates a new dispatch source object that monitors the system for changes in the memory pressure condition.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func makeMemoryPressureSource(
    eventMask: DispatchSource.MemoryPressureEvent,
    queue: DispatchQueue? = nil
) -> any DispatchSourceMemoryPressure
```

## Parameters 

`eventMask`  

The set of events you want to monitor. For a list of possible values, see DispatchSource.MemoryPressureEvent.

`queue`  

The dispatch queue to use when executing the installed handlers.

## Return Value

A dispatch source object that conforms to the DispatchSourceMemoryPressure protocol.

## Discussion

After creating the dispatch source, use the methods of the DispatchSourceProtocol protocol to install the event handlers you need. The returned dispatch source is in the inactive state initially. When you are ready to begin processing events, call its activate() method.

## See Also

### Creating a Memory Pressure Source

protocol DispatchSourceMemoryPressure

A dispatch source that monitors the system for changes in the memory pressure condition.

struct MemoryPressureEvent

Memory pressure events.

