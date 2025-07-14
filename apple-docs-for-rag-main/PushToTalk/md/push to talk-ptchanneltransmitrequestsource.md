

- Push to Talk
-  PTChannelTransmitRequestSource 

Enumeration

# PTChannelTransmitRequestSource

Identifies the type that indicates the transmission request source.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum PTChannelTransmitRequestSource
```

## Topics

### Transmission sources

case userRequest

A transmission request that indicates the user pressed the transmit button in the system user interface.

case developerRequest

A transmission request that indicates the app calls the begin transmission method.

case handsfreeButton

A transmission request that indicates a user pressed a button on a hands-free device.

case unknown

A transmission request that indicates an unknown reason.

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

enum PTChannelLeaveReason

Identifies the type that indicates the leave reason.

