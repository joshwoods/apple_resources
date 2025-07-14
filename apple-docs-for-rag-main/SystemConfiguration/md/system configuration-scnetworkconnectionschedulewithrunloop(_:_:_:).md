

- System Configuration
-  SCNetworkConnectionScheduleWithRunLoop(\_:\_:\_:) 

Function

# SCNetworkConnectionScheduleWithRunLoop(\_:\_:\_:)

Schedules the specified connection with the specified run loop.

macOS 10.3+

``` source
func SCNetworkConnectionScheduleWithRunLoop(
    _ connection: SCNetworkConnection,
    _ runLoop: CFRunLoop,
    _ runLoopMode: CFString
) -> Bool
```

## Parameters 

`connection`  

The network connection to schedule.

`runLoop`  

The run loop with which to schedule the network connection.

`runLoopMode`  

The run loop mode.

## Return Value

`TRUE` if the connection is scheduled successfully; `FALSE` (use the SCError() function to retrieve the specific error).

## See Also

### Scheduling a Connection Reference on a Run Loop

func SCNetworkConnectionUnscheduleFromRunLoop(SCNetworkConnection, CFRunLoop, CFString) -> Bool

Unschedules the specified connection from the specified run loop.

