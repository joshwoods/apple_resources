

- Push to Talk
-  PTChannelJoinReason 

Enumeration

# PTChannelJoinReason

Identifies the type that indicates the join reason.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum PTChannelJoinReason
```

## Topics

### Join reasons

case developerRequest

A join reason that indicates the app calls the join channel method while in the foreground.

case channelRestoration

A join reason that indicates the app rejoined a channel through channel restoration.

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

enum PTTransmissionMode

Identifies the type of audio transmission modes.

enum PTServiceStatus

Identifies the type that indicates the status of the service.

enum PTChannelLeaveReason

Identifies the type that indicates the leave reason.

enum PTChannelTransmitRequestSource

Identifies the type that indicates the transmission request source.

