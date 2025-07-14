

- Core Foundation
-  CFSocketConnectToAddress(\_:\_:\_:) 

Function

# CFSocketConnectToAddress(\_:\_:\_:)

Opens a connection to a remote socket.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketConnectToAddress(
    _ s: CFSocket!,
    _ address: CFData!,
    _ timeout: CFTimeInterval
) -> CFSocketError
```

## Parameters 

`s`  

The CFSocket object with which to connect to `address`.

`address`  

A CFData object containing a `struct sockaddr` appropriate for the protocol family of `s` (`struct sockaddr_in` or `struct sockaddr_in6`, for example), indicating the remote address to which to connect. This data object is used only for the duration of the function call.

`timeout`  

The time to wait for a connection to succeed. If a negative value is used, this function does not wait for the connection and instead lets the connection attempt happen in the background. If `s` requested a `kCFSocketConnectCallBack`, you will receive a callback when the background connection succeeds or fails.

## Return Value

An error code indicating success or failure of the connection attempt.

## See Also

### Using Sockets

func CFSocketCreateRunLoopSource(CFAllocator!, CFSocket!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFSocket object.

func CFSocketGetTypeID() -> CFTypeID

Returns the type identifier for the CFSocket opaque type.

func CFSocketInvalidate(CFSocket!)

Invalidates a CFSocket object, stopping it from sending or receiving any more messages.

func CFSocketIsValid(CFSocket!) -> Bool

Returns a Boolean value that indicates whether a CFSocket object is valid and able to send or receive messages.

func CFSocketSendData(CFSocket!, CFData!, CFData!, CFTimeInterval) -> CFSocketError

Sends data over a CFSocket object.

