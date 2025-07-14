

- System
- Errno
-  notSupportedOnSocket 

Type Property

# notSupportedOnSocket

Operation not supported on socket.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var notSupportedOnSocket: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The attempted operation isn’t supported for the type of socket referenced; for example, trying to accept a connection on a datagram socket.

The corresponding C error is `EOPNOTSUPP`.

## See Also

### Network Socket Errors

static var notSocket: Errno

A socket operation was performed on something that isn’t a socket.

static var socketIsConnected: Errno

Socket is already connected.

static var socketNotConnected: Errno

Socket is not connected.

static var socketShutdown: Errno

Can’t send after socket shutdown.

static var socketTypeNotSupported: Errno

Socket type not supported.

