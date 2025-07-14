

- Core Foundation
-  CFSocketEnableCallBacks(\_:\_:) 

Function

# CFSocketEnableCallBacks(\_:\_:)

Enables the callback function of a CFSocket object for certain types of socket activity.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketEnableCallBacks(
    _ s: CFSocket!,
    _ callBackTypes: CFOptionFlags
)
```

## Parameters 

`s`  

The CFSocket object to modify.

`callBackTypes`  

A bitwise-OR combination of CFSocket activity types that should cause the callback function of `s` to be called. See CFSocketCallBackType for a list of callback types.

## Discussion

If a callback type is not automatically reenabled, you can use this function to enable the callback (once).

This call does not affect whether the callback type will be automatically reenabled in the future; use CFSocketSetSocketFlags(_:_:) if you want to set a callback type to be reenabled automatically.

Be sure to enable only callback types that your CFSocket object actually possesses and has requested when creating the CFSocket object; the result of enabling other callback types is undefined.

## See Also

### Configuring Sockets

func CFSocketCopyAddress(CFSocket!) -> CFData!

Returns the local address of a CFSocket object.

func CFSocketCopyPeerAddress(CFSocket!) -> CFData!

Returns the remote address to which a CFSocket object is connected.

func CFSocketDisableCallBacks(CFSocket!, CFOptionFlags)

Disables the callback function of a CFSocket object for certain types of socket activity.

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

