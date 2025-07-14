

- Core Foundation
-  CFSocketGetNative(\_:) 

Function

# CFSocketGetNative(\_:)

Returns the native socket associated with a CFSocket object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketGetNative(_ s: CFSocket!) -> CFSocketNativeHandle
```

## Parameters 

`s`  

The CFSocket object to examine.

## Return Value

The native socket associated with `s`. If `s` has been invalidated, returns `-1`, `INVALID_SOCKET`.

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

func CFSocketGetSocketFlags(CFSocket!) -> CFOptionFlags

Returns flags that control certain behaviors of a CFSocket object.

func CFSocketSetAddress(CFSocket!, CFData!) -> CFSocketError

Binds a local address to a CFSocket object and configures it for listening.

func CFSocketSetSocketFlags(CFSocket!, CFOptionFlags)

Sets flags that control certain behaviors of a CFSocket object.

