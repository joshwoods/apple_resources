

- CloudKit
- CKShare
- CKShare.Participant
-  acceptanceStatus 

Instance Property

# acceptanceStatus

The current state of the user’s acceptance of the share.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var acceptanceStatus: CKShare.ParticipantAcceptanceStatus { get }
```

## Discussion

This property contains the current state of the participant’s acceptance of the share. For a list of possible values, see CKShare.ParticipantAcceptanceStatus.

## See Also

### Accessing the Participant’s Status

typealias AcceptanceStatus

A type that represents the acceptance status of the participant.

enum ParticipantAcceptanceStatus

Constants that represent the status of a participant.

