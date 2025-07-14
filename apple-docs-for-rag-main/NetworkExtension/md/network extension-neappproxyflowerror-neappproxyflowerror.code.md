

- Network Extension
- NEAppProxyFlowError
-  NEAppProxyFlowError.Code 

Enumeration

# NEAppProxyFlowError.Code

Error codes that the app proxy flow API declares.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Code
```

## Topics

### Error Codes

case notConnected

The flow is not fully opened.

case peerReset

The remote peer closed the flow.

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

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct NEAppProxyFlowError

An error that the app proxy flow encounters.

let NEAppProxyErrorDomain: String

The domain used for app proxy errors.

struct NEAppProxyFlowError

An error that the app proxy flow encounters.

