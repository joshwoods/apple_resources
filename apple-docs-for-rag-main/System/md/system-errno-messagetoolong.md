

- System
- Errno
-  messageTooLong 

Type Property

# messageTooLong

Message too long.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var messageTooLong: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A message sent on a socket was larger than the internal message buffer or some other network limit.

The corresponding C error is `EMSGSIZE`.

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

static var notSupported: Errno

Not supported.

static var timedOut: Errno

Operation timed out.

