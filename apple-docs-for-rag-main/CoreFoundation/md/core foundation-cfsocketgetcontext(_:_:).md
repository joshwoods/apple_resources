

- Core Foundation
-  CFSocketGetContext(\_:\_:) 

Function

# CFSocketGetContext(\_:\_:)

Returns the context information for a CFSocket object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketGetContext(
    _ s: CFSocket!,
    _ context: UnsafeMutablePointer!
)
```

## Parameters 

`s`  

The CFSocket object to examine.

`context`  

A pointer to the structure into which the context information for `s` is to be copied. The information being returned is usually the same information you passed to CFSocketCreate(_:_:_:_:_:_:_:), CFSocketCreateConnectedToSocketSignature(_:_:_:_:_:_:), CFSocketCreateWithNative(_:_:_:_:_:), or CFSocketCreateWithSocketSignature(_:_:_:_:_:) when creating the CFSocket object. However, if CFSocketCreateWithNative(_:_:_:_:_:) returned a cached CFSocket object instead of creating a new object, `context` is filled with information from the original CFSocket object instead of the information you passed to the function.

## Discussion

The context version number for CFSocket is currently 0. Before calling this function, you need to initialize the `version` member of `context` to 0.

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

func CFSocketGetNative(CFSocket!) -> CFSocketNativeHandle

Returns the native socket associated with a CFSocket object.

func CFSocketGetSocketFlags(CFSocket!) -> CFOptionFlags

Returns flags that control certain behaviors of a CFSocket object.

func CFSocketSetAddress(CFSocket!, CFData!) -> CFSocketError

Binds a local address to a CFSocket object and configures it for listening.

func CFSocketSetSocketFlags(CFSocket!, CFOptionFlags)

Sets flags that control certain behaviors of a CFSocket object.

