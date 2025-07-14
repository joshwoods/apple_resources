

- Core Foundation
-  CFSocketIsValid(\_:) 

Function

# CFSocketIsValid(\_:)

Returns a Boolean value that indicates whether a CFSocket object is valid and able to send or receive messages.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketIsValid(_ s: CFSocket!) -> Bool
```

## Parameters 

`s`  

The CFSocket object to examine.

## Return Value

`true` if `s` can be used for communication, otherwise `false`.

## See Also

### Using Sockets

func CFSocketConnectToAddress(CFSocket!, CFData!, CFTimeInterval) -> CFSocketError

Opens a connection to a remote socket.

func CFSocketCreateRunLoopSource(CFAllocator!, CFSocket!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFSocket object.

func CFSocketGetTypeID() -> CFTypeID

Returns the type identifier for the CFSocket opaque type.

func CFSocketInvalidate(CFSocket!)

Invalidates a CFSocket object, stopping it from sending or receiving any more messages.

func CFSocketSendData(CFSocket!, CFData!, CFData!, CFTimeInterval) -> CFSocketError

Sends data over a CFSocket object.

