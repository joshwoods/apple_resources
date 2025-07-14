

- Network Extension
- NEAppProxyFlowError
-  readAlreadyPending 

Type Property

# readAlreadyPending

A read operation on the flow is already pending.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
static var readAlreadyPending: NEAppProxyFlowError.Code { get }
```

## See Also

### Error codes

static var notConnected: NEAppProxyFlowError.Code

The flow is not fully opened.

static var peerReset: NEAppProxyFlowError.Code

The remote peer closed the flow.

static var hostUnreachable: NEAppProxyFlowError.Code

An attempt to reach the remote endpoint of the flow failed.

static var invalidArgument: NEAppProxyFlowError.Code

A proxy flow method received an invalid argument.

static var aborted: NEAppProxyFlowError.Code

The flow was aborted.

static var refused: NEAppProxyFlowError.Code

Connecting the flow to its remote endpoint failed.

static var timedOut: NEAppProxyFlowError.Code

The flow timed out.

static var `internal`: NEAppProxyFlowError.Code

An internal error occurred while handling the flow.

static var datagramTooLarge: NEAppProxyFlowError.Code

A caller attempted to write a datagram that was larger than the socket’s receive window.

