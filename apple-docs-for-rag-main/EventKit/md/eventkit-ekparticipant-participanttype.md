

- EventKit
- EKParticipant
-  participantType 

Instance Property

# participantType

The participant’s type.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var participantType: EKParticipantType { get }
```

## See Also

### Related Documentation

enum EKParticipantType

The type of participant.

### Accessing Participant Properties

var isCurrentUser: Bool

A Boolean value indicating whether this participant represents the owner of this account.

var name: String?

The participant’s name.

var participantRole: EKParticipantRole

The participant’s role in the event.

var participantStatus: EKParticipantStatus

The participant’s attendance status.

var url: URL

The URL representing this participant.

var contactPredicate: NSPredicate

A predicate to use with the Contacts framework to retrieve the corresponding contact instance.

