

- Push to Talk
-  PTTransmissionMode 

Enumeration

# PTTransmissionMode

Identifies the type of audio transmission modes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum PTTransmissionMode
```

## Topics

### Modes

case fullDuplex

A type that indicates a participant can simultaneously receive and transmit audio.

case halfDuplex

A type that indicates a participant can’t simultaneously receive and transmit audio.

case listenOnly

A type that indicates a participant can only receive audio.

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

### Channel management

protocol PTChannelManagerDelegate

A type that represents your life cycle of a channel manager.

enum PTServiceStatus

Identifies the type that indicates the status of the service.

enum PTChannelJoinReason

Identifies the type that indicates the join reason.

enum PTChannelLeaveReason

Identifies the type that indicates the leave reason.

enum PTChannelTransmitRequestSource

Identifies the type that indicates the transmission request source.

