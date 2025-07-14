

- System
- Errno
-  socketShutdown 

Type Property

# socketShutdown

Can’t send after socket shutdown.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var socketShutdown: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A request to send data wasn’t permitted because the socket had already been shut down with a previous `shutdown(2)` call.

The corresponding C error is `ESHUTDOWN`.

## See Also

### Network Socket Errors

static var notSocket: Errno

A socket operation was performed on something that isn’t a socket.

static var notSupportedOnSocket: Errno

Operation not supported on socket.

static var socketIsConnected: Errno

Socket is already connected.

static var socketNotConnected: Errno

Socket is not connected.

static var socketTypeNotSupported: Errno

Socket type not supported.

