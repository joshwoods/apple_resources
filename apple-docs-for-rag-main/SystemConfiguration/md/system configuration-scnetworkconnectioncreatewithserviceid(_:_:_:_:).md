

- System Configuration
-  SCNetworkConnectionCreateWithServiceID(\_:\_:\_:\_:) 

Function

# SCNetworkConnectionCreateWithServiceID(\_:\_:\_:\_:)

Creates a new connection reference to use for getting the status or for connecting or disconnecting the associated service.

macOS 10.3+

``` source
func SCNetworkConnectionCreateWithServiceID(
    _ allocator: CFAllocator?,
    _ serviceID: CFString,
    _ callout: SCNetworkConnectionCallBack?,
    _ context: UnsafeMutablePointer?
) -> SCNetworkConnection?
```

## Parameters 

`allocator`  

The allocator that should be used to allocate memory for the connection structure. This parameter may be `NULL`, in which case the current default allocator is used. If this reference is not a valid allocator, the behavior is undefined.

`serviceID`  

The service identifier of the connection. This value uniquely identifies service in the system configuration database.

`callout`  

The function to be called when the status of the connection changes. If this parameter is `NULL`, the application receives notifications of status change and will need to poll for updates.

`context`  

User-specified data associated with the connection.

## Return Value

A reference to a new network connection.

