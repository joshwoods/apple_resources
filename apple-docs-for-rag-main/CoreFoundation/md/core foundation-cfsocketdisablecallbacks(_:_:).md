

- Core Foundation
-  CFSocketDisableCallBacks(\_:\_:) 

Function

# CFSocketDisableCallBacks(\_:\_:)

Disables the callback function of a CFSocket object for certain types of socket activity.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketDisableCallBacks(
    _ s: CFSocket!,
    _ callBackTypes: CFOptionFlags
)
```

## Parameters 

`s`  

The CFSocket object to modify.

`callBackTypes`  

A bitwise-OR combination of CFSocket activity types that should not cause the callback function of `s` to be called. See CFSocketCallBackType for a list of callback types.

## Discussion

If you no longer want certain types of callbacks that you requested when creating `s`, you can use this function to temporarily disable the callback. Use CFSocketEnableCallBacks(_:_:) to reenable a callback type.

## See Also

### Configuring Sockets

func CFSocketCopyAddress(CFSocket!) -> CFData!

Returns the local address of a CFSocket object.

func CFSocketCopyPeerAddress(CFSocket!) -> CFData!

Returns the remote address to which a CFSocket object is connected.

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

