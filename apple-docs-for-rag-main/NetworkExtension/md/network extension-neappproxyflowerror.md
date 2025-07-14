

- Network Extension
-  NEAppProxyFlowError 

Structure

# NEAppProxyFlowError

An error that the app proxy flow encounters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NEAppProxyFlowError
```

## Topics

### Accessing error properties

enum Code

Error codes that the app proxy flow API declares.

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

static var readAlreadyPending: NEAppProxyFlowError.Code

A read operation on the flow is already pending.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

let NEAppProxyErrorDomain: String

The domain used for app proxy errors.

enum Code

Error codes that the app proxy flow API declares.

