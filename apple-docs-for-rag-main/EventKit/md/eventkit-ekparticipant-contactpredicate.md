

- EventKit
- EKParticipant
-  contactPredicate 

Instance Property

# contactPredicate

A predicate to use with the Contacts framework to retrieve the corresponding contact instance.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var contactPredicate: NSPredicate { get }
```

## Discussion

Use this property to get a predicate that you can use with a CNContactStore to fetch a CNContact instance for this participant, if one exists.

## See Also

### Accessing Participant Properties

var isCurrentUser: Bool

A Boolean value indicating whether this participant represents the owner of this account.

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

