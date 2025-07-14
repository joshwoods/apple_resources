

- Push to Talk
-  PTChannelLeaveReason 

Enumeration

# PTChannelLeaveReason

Identifies the type that indicates the leave reason.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum PTChannelLeaveReason
```

## Topics

### Leave reasons

case userRequest

A leave reason that indicates a user pressed the leave button in the user interface.

case developerRequest

A leave reason that indicates the app calls the leave channel method.

case systemPolicy

A leave reason that indicates a new device restriction is in effect.

case unknown

A leave reason that indicates an unknown reason.

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

enum PTChannelJoinReason

Identifies the type that indicates the join reason.

enum PTChannelTransmitRequestSource

Identifies the type that indicates the transmission request source.

