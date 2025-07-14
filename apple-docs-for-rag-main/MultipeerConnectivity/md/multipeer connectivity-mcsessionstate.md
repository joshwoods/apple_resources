

- Multipeer Connectivity
-  MCSessionState 

Enumeration

# MCSessionState

Indicates the current state of a given peer within a session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
enum MCSessionState
```

## Topics

### Constants

case notConnected

The peer is not (or is no longer) in this session.

case connecting

A connection to the peer is currently being established.

case connected

The peer is connected to this session.

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

### Constants

enum MCSessionSendDataMode

Indicates whether delivery of data should be guaranteed.

enum MCEncryptionPreference

Indicates whether a session should use encryption when communicating with nearby peers.

enum Code

Error codes found in MCErrorDomain error domain `NSError` objects returned by methods in the Multipeer Connectivity framework.

Multipeer Connectivity Error Domain

The error domain for errors specific to Multipeer Connectivity.

Minimum and Maximum Supported Peers

Constants that define the minimum and maximum number of peers supported in a session.

