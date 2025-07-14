

- System Configuration
-  SCNetworkConnectionStop(\_:\_:) 

Function

# SCNetworkConnectionStop(\_:\_:)

Stops the connection process for the specified network connection.

macOS 10.3+

``` source
func SCNetworkConnectionStop(
    _ connection: SCNetworkConnection,
    _ forceDisconnect: Bool
) -> Bool
```

## Parameters 

`connection`  

The network connection to stop.

`forceDisconnect`  

Pass `TRUE` to stop the connection regardless of other applications that might have interest in it.

## Return Value

`TRUE` if the disconnection request succeeded; `FALSE` (use the SCError() function to retrieve the specific error).

## See Also

### Starting and Stopping a Connection

func SCNetworkConnectionStart(SCNetworkConnection, CFDictionary?, Bool) -> Bool

Starts the connection process for the specified network connection.

