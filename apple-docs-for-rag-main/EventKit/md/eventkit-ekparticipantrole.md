

- EventKit
-  EKParticipantRole 

Enumeration

# EKParticipantRole

The participant’s role for an event.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKParticipantRole
```

## Topics

### Constants

case unknown

The participant’s role is unknown.

case required

The participant’s attendance is required.

case optional

The participant’s attendance is optional.

case chair

The participant is the chair of the event.

case nonParticipant

The participant does not have an active role in the event.

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

enum EKParticipantType

The type of participant.

enum EKParticipantStatus

The participant’s attendance status for an event.

enum EKParticipantScheduleStatus

The participant’s scheduled status.

