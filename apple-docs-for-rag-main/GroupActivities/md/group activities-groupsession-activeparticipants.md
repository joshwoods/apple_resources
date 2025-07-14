

- Group Activities
- GroupSession
-  activeParticipants 

Instance Property

# activeParticipants

The set of participants currently engaged in the activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
@Published
final var activeParticipants: Set { get }
```

## Mentioned in 

Joining and managing a shared activity

## Discussion

This property reflects the set of people invited to a group session and currently engaged in the shared activity on their device. Members who join the conversation over FaceTime but don’t join the shared activity aren’t active participants. As people join or leave the activity, the session object updates the set of active participants. To detect changes to this property, configure a subscriber.

Each Participant object corresponds to a joined session on a device. If a single person joins the activity from two devices simultaneously, the set contains a separate Participant object for each device.

## See Also

### Getting the participants

var localParticipant: Participant

The participant on the current device.

