

- EventKit
-  EKParticipantStatus 

Enumeration

# EKParticipantStatus

The participant’s attendance status for an event.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKParticipantStatus
```

## Topics

### Constants

case unknown

The participant’s attendance status is unknown.

case pending

The participant has yet to respond to the event.

case accepted

The participant has accepted the event.

case declined

The participant has declined the event.

case tentative

The participant’s attendance status is tentative.

case delegated

The participant has delegated attendance to another participant.

case completed

The participant’s event has completed.

case inProcess

The participant’s event is currently in process.

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

### Defining Participants

enum EKParticipantRole

The participant’s role for an event.

enum EKParticipantType

The type of participant.

enum EKParticipantScheduleStatus

The participant’s scheduled status.

