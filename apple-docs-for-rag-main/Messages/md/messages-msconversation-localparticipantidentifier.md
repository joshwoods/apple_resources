

- Messages
- MSConversation
-  localParticipantIdentifier 

Instance Property

# localParticipantIdentifier

A UUID that identifies the user on this device.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
var localParticipantIdentifier: UUID { get }
```

## Discussion

This UUID is scoped to this device. It remains stable as long as the extension is enabled. If the extension is disabled and reenabled, or if the containing app is removed and reinstalled, the UUID for the local participant changes.

## See Also

### Accessing Participants

var remoteParticipantIdentifiers: [UUID]

An array of UUIDs representing the remote participants in this conversation.

