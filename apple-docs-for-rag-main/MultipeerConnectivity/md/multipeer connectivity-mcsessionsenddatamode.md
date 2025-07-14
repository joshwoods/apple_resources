

- Multipeer Connectivity
-  MCSessionSendDataMode 

Enumeration

# MCSessionSendDataMode

Indicates whether delivery of data should be guaranteed.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
enum MCSessionSendDataMode
```

## Topics

### Constants

case reliable

The framework should guarantee delivery of each message, enqueueing and retransmitting data as needed, and ensuring in-order delivery.

case unreliable

Messages to peers should be sent immediately without socket-level queueing. If a message cannot be sent immediately, it should be dropped. The order of messages is not guaranteed.

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

enum MCSessionState

Indicates the current state of a given peer within a session.

enum MCEncryptionPreference

Indicates whether a session should use encryption when communicating with nearby peers.

enum Code

Error codes found in MCErrorDomain error domain `NSError` objects returned by methods in the Multipeer Connectivity framework.

Multipeer Connectivity Error Domain

The error domain for errors specific to Multipeer Connectivity.

Minimum and Maximum Supported Peers

Constants that define the minimum and maximum number of peers supported in a session.

