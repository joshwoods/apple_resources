

- Core Foundation
-  CFSocketInvalidate(\_:) 

Function

# CFSocketInvalidate(\_:)

Invalidates a CFSocket object, stopping it from sending or receiving any more messages.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketInvalidate(_ s: CFSocket!)
```

## Parameters 

`s`  

The CFSocket object to invalidate.

## Discussion

You should always invalidate a socket object when you are through using it. Invalidating a CFSocket object prevents the object from sending or receiving any more messages, but does not release the socket object itself.

If a run loop source was created for `s`, the run loop source is invalidated.

If a release callback was specified in CFSocketContext object, this function calls it to release the object in the `info` field (which was provided when `s` was created).

By default, this call closes the underlying socket. If you have explicitly cleared the `kCFSocketCloseOnInvalidate` flag by calling CFSocketSetSocketFlags(_:_:), you must close the socket yourself *after* calling this function.

## See Also

### Using Sockets

func CFSocketConnectToAddress(CFSocket!, CFData!, CFTimeInterval) -> CFSocketError

Opens a connection to a remote socket.

func CFSocketCreateRunLoopSource(CFAllocator!, CFSocket!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFSocket object.

func CFSocketGetTypeID() -> CFTypeID

Returns the type identifier for the CFSocket opaque type.

func CFSocketIsValid(CFSocket!) -> Bool

Returns a Boolean value that indicates whether a CFSocket object is valid and able to send or receive messages.

func CFSocketSendData(CFSocket!, CFData!, CFData!, CFTimeInterval) -> CFSocketError

Sends data over a CFSocket object.

