

- Core Foundation
-  CFSocketGetTypeID() 

Function

# CFSocketGetTypeID()

Returns the type identifier for the CFSocket opaque type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketGetTypeID() -> CFTypeID
```

## Return Value

The type identifier for the CFSocket opaque type.

## See Also

### Using Sockets

func CFSocketConnectToAddress(CFSocket!, CFData!, CFTimeInterval) -> CFSocketError

Opens a connection to a remote socket.

func CFSocketCreateRunLoopSource(CFAllocator!, CFSocket!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFSocket object.

func CFSocketInvalidate(CFSocket!)

Invalidates a CFSocket object, stopping it from sending or receiving any more messages.

func CFSocketIsValid(CFSocket!) -> Bool

Returns a Boolean value that indicates whether a CFSocket object is valid and able to send or receive messages.

func CFSocketSendData(CFSocket!, CFData!, CFData!, CFTimeInterval) -> CFSocketError

Sends data over a CFSocket object.

