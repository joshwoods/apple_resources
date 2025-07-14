

- Push to Talk
-  PTServiceStatus 

Enumeration

# PTServiceStatus

Identifies the type that indicates the status of the service.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum PTServiceStatus
```

## Topics

### Statuses

case ready

A type that indicates the service is available for use.

case connecting

A type that indicates the service is attempting to establish a connection.

case unavailable

A type that indicates the service is unavailable and needs to be re-established.

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

enum PTChannelJoinReason

Identifies the type that indicates the join reason.

enum PTChannelLeaveReason

Identifies the type that indicates the leave reason.

enum PTChannelTransmitRequestSource

Identifies the type that indicates the transmission request source.

