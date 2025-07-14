

- EventKit
-  EKParticipantScheduleStatus 

Enumeration

# EKParticipantScheduleStatus

The participant’s scheduled status.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKParticipantScheduleStatus
```

## Topics

### Constants

case none

The invitation hasn’t been sent yet.

case pending

The invitation is in the process of being sent.

case sent

The invitation has been sent, but it’s unclear if it was successfully delivered.

case delivered

The invitation has been sent and successfully delivered.

case recipientNotRecognized

The invitation wasn’t delivered because the source doesn’t recognize the recipient.

case noPrivileges

The invitation wasn’t delivered because of insufficient privileges.

case deliveryFailed

The invitation wasn’t delivered due to a temporary failure.

case cannotDeliver

The invitation wasn’t delivered because the system is unsure of how to deliver it.

case recipientNotAllowed

The invitation wasn’t delivered because scheduling with the participant isn’t allowed.

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

enum EKParticipantStatus

The participant’s attendance status for an event.

