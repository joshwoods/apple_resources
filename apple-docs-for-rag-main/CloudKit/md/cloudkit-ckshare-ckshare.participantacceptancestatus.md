

- CloudKit
- CKShare
-  CKShare.ParticipantAcceptanceStatus 

Enumeration

# CKShare.ParticipantAcceptanceStatus

Constants that represent the status of a participant.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum ParticipantAcceptanceStatus
```

## Topics

### Constants

case unknown

The participant’s status is unknown.

case pending

The participant’s acceptance of the share request is pending.

case accepted

The participant accepted the share request.

case removed

The system removed the participant from the share.

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

### Accessing the Participant’s Status

var acceptanceStatus: CKShare.ParticipantAcceptanceStatus

The current state of the user’s acceptance of the share.

typealias AcceptanceStatus

A type that represents the acceptance status of the participant.

