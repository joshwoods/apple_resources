

- EventKit
- EKParticipant
-  participantRole 

Instance Property

# participantRole

The participant’s role in the event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var participantRole: EKParticipantRole { get }
```

## See Also

### Related Documentation

enum EKParticipantRole

The participant’s role for an event.

### Accessing Participant Properties

var isCurrentUser: Bool

A Boolean value indicating whether this participant represents the owner of this account.

var name: String?

The participant’s name.

var participantStatus: EKParticipantStatus

The participant’s attendance status.

var participantType: EKParticipantType

The participant’s type.

var url: URL

The URL representing this participant.

var contactPredicate: NSPredicate

A predicate to use with the Contacts framework to retrieve the corresponding contact instance.

