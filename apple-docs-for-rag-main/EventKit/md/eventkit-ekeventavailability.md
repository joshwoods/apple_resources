

- EventKit
-  EKEventAvailability 

Enumeration

# EKEventAvailability

The event’s availability setting for scheduling purposes.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKEventAvailability
```

## Topics

### Constants

case notSupported

Availability settings are not supported by the event’s calendar.

case busy

The event has a busy availability setting.

case free

The event has a free availability setting.

case tentative

The event has a tentative availability setting.

case unavailable

The event has an unavailable availability setting.

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

### Scheduling Events

enum EKEventStatus

The event’s status.

