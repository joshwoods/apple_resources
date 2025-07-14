

- Core Foundation
-  CFSocketGetSocketFlags(\_:) 

Function

# CFSocketGetSocketFlags(\_:)

Returns flags that control certain behaviors of a CFSocket object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketGetSocketFlags(_ s: CFSocket!) -> CFOptionFlags
```

## Parameters 

`s`  

The CFSocket to examine.

## Return Value

A bitwise-OR combination of flags controlling the behavior of `s`. See CFSocket Flags for the list of available flags.

## Discussion

See CFSocketSetSocketFlags(_:_:) for details on what the flags of a CFSocket mean.

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

func CFSocketSetAddress(CFSocket!, CFData!) -> CFSocketError

Binds a local address to a CFSocket object and configures it for listening.

func CFSocketSetSocketFlags(CFSocket!, CFOptionFlags)

Sets flags that control certain behaviors of a CFSocket object.

