

- System
- Errno
-  notSupported 

Type Property

# notSupported

Not supported.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var notSupported: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The attempted operation isn’t supported for the type of object referenced.

The corresponding C error is `ENOTSUP`.

## See Also

### Network Errors

static var connectionAbort: Errno

Software caused a connection abort.

static var connectionRefused: Errno

Connection refused.

static var connectionReset: Errno

Connection reset by peer.

static var hostIsDown: Errno

The host is down.

static var messageTooLong: Errno

Message too long.

static var networkDown: Errno

Network is down.

static var networkReset: Errno

Network dropped connection on reset.

static var networkUnreachable: Errno

Network is unreachable.

static var noBufferSpace: Errno

No buffer space available.

static var noRouteToHost: Errno

No route to host.

static var timedOut: Errno

Operation timed out.

