

- EventKit
- EKParticipant
-  isCurrentUser 

Instance Property

# isCurrentUser

A Boolean value indicating whether this participant represents the owner of this account.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+watchOS 2.0+

``` source
var isCurrentUser: Bool { get }
```

## See Also

### Related Documentation

Calendar and Reminders Programming Guide

### Accessing Participant Properties

var name: String?

The participant’s name.

var participantRole: EKParticipantRole

The participant’s role in the event.

var participantStatus: EKParticipantStatus

The participant’s attendance status.

var participantType: EKParticipantType

The participant’s type.

var url: URL

The URL representing this participant.

var contactPredicate: NSPredicate

A predicate to use with the Contacts framework to retrieve the corresponding contact instance.

