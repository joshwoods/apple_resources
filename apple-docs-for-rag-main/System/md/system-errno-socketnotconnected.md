

- System
- Errno
-  socketNotConnected 

Type Property

# socketNotConnected

Socket is not connected.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var socketNotConnected: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A request to send or receive data wasn’t permitted because the socket wasn’t connected and, when sending on a datagram socket, no address was supplied.

The corresponding C error is `ENOTCONN`.

## See Also

### Network Socket Errors

static var notSocket: Errno

A socket operation was performed on something that isn’t a socket.

static var notSupportedOnSocket: Errno

Operation not supported on socket.

static var socketIsConnected: Errno

Socket is already connected.

static var socketShutdown: Errno

Can’t send after socket shutdown.

static var socketTypeNotSupported: Errno

Socket type not supported.

