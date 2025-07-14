

- System
- Errno
-  socketTypeNotSupported 

Type Property

# socketTypeNotSupported

Socket type not supported.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var socketTypeNotSupported: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

Support for the socket type hasn’t been configured into the system or no implementation for it exists.

The corresponding C error is `ESOCKTNOSUPPORT`.

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

static var socketShutdown: Errno

Can’t send after socket shutdown.

