

- Network Extension
- NEAppProxyFlowError
- NEAppProxyFlowError.Code
-  NEAppProxyFlowError.Code.peerReset 

Case

# NEAppProxyFlowError.Code.peerReset

The remote peer closed the flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case peerReset
```

## See Also

### Error Codes

case notConnected

The flow is not fully opened.

case hostUnreachable

An attempt to reach the remote endpoint of the flow failed.

case invalidArgument

A proxy flow method received an invalid argument.

case aborted

The flow was aborted.

case refused

Connecting the flow to its remote endpoint failed.

case timedOut

The flow timed out.

case `internal`

An internal error occurred while handling the flow.

case datagramTooLarge

A caller attempted to write a datagram that was larger than the socket’s receive window.

case readAlreadyPending

A read operation on the flow is already pending.

