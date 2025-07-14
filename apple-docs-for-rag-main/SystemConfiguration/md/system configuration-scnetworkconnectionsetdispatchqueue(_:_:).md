

- System Configuration
-  SCNetworkConnectionSetDispatchQueue(\_:\_:) 

Function

# SCNetworkConnectionSetDispatchQueue(\_:\_:)

Specifies a dispatch queue to use for the connection’s callback function and enables notifications.

macOS 10.6+

``` source
func SCNetworkConnectionSetDispatchQueue(
    _ connection: SCNetworkConnection,
    _ queue: dispatch_queue_t?
) -> Bool
```

## Parameters 

`connection`  

The network connection to notify.

`queue`  

The queue on which to run the connection’s callback function. Pass `NULL` to disable notifications and release the queue.

## Return Value

`TRUE` if successful; otherwise, `FALSE` (use the SCError() function to retrieve the specific error).

