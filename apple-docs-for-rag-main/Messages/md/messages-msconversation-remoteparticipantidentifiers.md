

- Messages
- MSConversation
-  remoteParticipantIdentifiers 

Instance Property

# remoteParticipantIdentifiers

An array of UUIDs representing the remote participants in this conversation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
var remoteParticipantIdentifiers: [UUID] { get }
```

## Discussion

These UUIDs are scoped to this device. They remain stable as long as the extension is enabled. If the extension is disabled and reenabled, or if the containing app is removed and reinstalled, the UUIDs for remote participants change.

## See Also

### Accessing Participants

var localParticipantIdentifier: UUID

A UUID that identifies the user on this device.

