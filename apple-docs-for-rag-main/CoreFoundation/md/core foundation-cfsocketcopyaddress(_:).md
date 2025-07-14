

- Core Foundation
-  CFSocketCopyAddress(\_:) 

Function

# CFSocketCopyAddress(\_:)

Returns the local address of a CFSocket object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketCopyAddress(_ s: CFSocket!) -> CFData!
```

## Parameters 

`s`  

The CFSocket object to examine.

## Return Value

The local address, stored as a `struct sockaddr` appropriate for the protocol family (`struct sockaddr_in` or `struct sockaddr_in6`, for example) in a CFData object, of `s`. Ownership follows the The Create Rule.

## See Also

### Configuring Sockets

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

func CFSocketSetAddress(CFSocket!, CFData!) -> CFSocketError

Binds a local address to a CFSocket object and configures it for listening.

func CFSocketSetSocketFlags(CFSocket!, CFOptionFlags)

Sets flags that control certain behaviors of a CFSocket object.

