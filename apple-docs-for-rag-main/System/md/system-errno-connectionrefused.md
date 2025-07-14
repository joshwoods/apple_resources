

- System
- Errno
-  connectionRefused 

Type Property

# connectionRefused

Connection refused.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var connectionRefused: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

No connection could be made because the target machine actively refused it. This usually results from trying to connect to a service that’s inactive on the foreign host.

The corresponding C error is `ECONNREFUSED`.

## See Also

### Network Errors

static var connectionAbort: Errno

Software caused a connection abort.

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

static var notSupported: Errno

Not supported.

static var timedOut: Errno

Operation timed out.

