

- System
- Errno
-  notSocket 

Type Property

# notSocket

A socket operation was performed on something that isn’t a socket.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var notSocket: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The corresponding C error is `ENOTSOCK`.

## See Also

### Network Socket Errors

static var notSupportedOnSocket: Errno

Operation not supported on socket.

static var socketIsConnected: Errno

Socket is already connected.

static var socketNotConnected: Errno

Socket is not connected.

static var socketShutdown: Errno

Can’t send after socket shutdown.

static var socketTypeNotSupported: Errno

Socket type not supported.

