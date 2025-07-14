

- Core Foundation
-  CFSocketSetAddress(\_:\_:) 

Function

# CFSocketSetAddress(\_:\_:)

Binds a local address to a CFSocket object and configures it for listening.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketSetAddress(
    _ s: CFSocket!,
    _ address: CFData!
) -> CFSocketError
```

## Parameters 

`s`  

The CFSocket object to modify.

`address`  

A CFData object containing a `struct sockaddr` appropriate for the protocol family of `s` (`struct sockaddr_in` or `struct sockaddr_in6`, for example). This data object is used only for the duration of the function call.

## Return Value

An error code indicating success or failure.

## Discussion

This function binds the socket by calling bind, and if the socket supports it, configures the socket for listening by calling listen with a backlog of 256.

Once `s` is bound to `address`, depending on the socket’s protocol, other processes and computers can connect to `s`.

## See Also

### Configuring Sockets

func CFSocketCopyAddress(CFSocket!) -> CFData!

Returns the local address of a CFSocket object.

func CFSocketCopyPeerAddress(CFSocket!) -> CFData!

Returns the remote address to which a CFSocket object is connected.

func CFSocketDisableCallBacks(CFSocket!, CFOptionFlags)

Disables the callback function of a CFSocket object for certain types of socket activity.

func CFSocketEnableCallBacks(CFSocket!, CFOptionFlags)

Enables the callback function of a CFSocket object for certain types of socket activity.

func CFSocketGetContext(CFSocket!, UnsafeMutablePointer&lt;CFSocketContext>!)

Returns the context information for a CFSocket object.

func CFSocketGetNative(CFSocket!) -> CFSocketNativeHandle

Returns the native socket associated with a CFSocket object.

func CFSocketGetSocketFlags(CFSocket!) -> CFOptionFlags

Returns flags that control certain behaviors of a CFSocket object.

func CFSocketSetSocketFlags(CFSocket!, CFOptionFlags)

Sets flags that control certain behaviors of a CFSocket object.

