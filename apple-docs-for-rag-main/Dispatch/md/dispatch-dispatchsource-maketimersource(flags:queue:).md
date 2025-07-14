

- Dispatch
- DispatchSource
-  makeTimerSource(flags:queue:) 

Type Method

# makeTimerSource(flags:queue:)

Creates a new dispatch source object for monitoring timer events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func makeTimerSource(
    flags: DispatchSource.TimerFlags = [],
    queue: DispatchQueue? = nil
) -> any DispatchSourceTimer
```

## Parameters 

`flags`  

Additional flags indicating the behavior of the timer. For a list of possible values, see DispatchSource.TimerFlags.

`queue`  

The dispatch queue to which to execute the installed handlers.

## Return Value

A dispatch source object that conforms to the DispatchSourceTimer protocol.

## Discussion

After creating the dispatch source, use the methods of the DispatchSourceProtocol protocol to install the event handlers you need. The returned dispatch source is in the inactive state initially. When you are ready to begin processing events, call its activate() method.

To schedule timers, use the methods of the DispatchSourceTimer protocol. You may schedule timers that fire once or fire multiple times. Each time the timer fires, the dispatch source calls your installed event handler.

## See Also

### Creating a Timer Source

protocol DispatchSourceTimer

A dispatch source that submits the event handler block based on a timer.

struct TimerFlags

Flags to use when configuring a timer dispatch source.

