

- System Configuration
-  SCNetworkConnectionUnscheduleFromRunLoop(\_:\_:\_:) 

Function

# SCNetworkConnectionUnscheduleFromRunLoop(\_:\_:\_:)

Unschedules the specified connection from the specified run loop.

macOS 10.3+

``` source
func SCNetworkConnectionUnscheduleFromRunLoop(
    _ connection: SCNetworkConnection,
    _ runLoop: CFRunLoop,
    _ runLoopMode: CFString
) -> Bool
```

## Parameters 

`connection`  

The network connection to unschedule.

`runLoop`  

The run loop from which to unschedule the network connection.

`runLoopMode`  

The run loop mode.

## Return Value

`TRUE` if the connection is unscheduled successfully; `FALSE` (use the SCError() function to retrieve the specific error).

## See Also

### Scheduling a Connection Reference on a Run Loop

func SCNetworkConnectionScheduleWithRunLoop(SCNetworkConnection, CFRunLoop, CFString) -> Bool

Schedules the specified connection with the specified run loop.

