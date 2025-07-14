

- Multipeer Connectivity
- MCError
-  MCError.Code 

Enumeration

# MCError.Code

Error codes found in MCErrorDomain error domain `NSError` objects returned by methods in the Multipeer Connectivity framework.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Constants

case unknown

An unknown error occurred.

case notConnected

Your app attempted to send data to a peer that is not connected.

case invalidParameter

Your app passed an invalid value as a parameter.

case unsupported

The operation is unsupported. For example, this error is returned if you call sendResource(at:withName:toPeer:withCompletionHandler:) with a URL that is neither a local file nor a web URL.

case timedOut

The connection attempt timed out.

case cancelled

The operation was cancelled by the user.

case unavailable

Multipeer connectivity is currently unavailable.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

