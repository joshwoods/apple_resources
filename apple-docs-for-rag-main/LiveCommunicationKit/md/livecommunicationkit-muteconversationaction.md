

- LiveCommunicationKit
-  MuteConversationAction 

Class

# MuteConversationAction

Mutes or unmutes `Conversation`. Muting a `Conversation` means that the local member will not be heard by any remote members.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final class MuteConversationAction
```

## Topics

### Initializers

init(conversationUUID: UUID, isMuted: Bool)

Creates a new `MuteConversationAction`.

### Instance Properties

let isMuted: Bool

Specifies if the `Conversation` should be muted or unmuted upon execution of this action.

## Relationships

### Inherits From

- ConversationAction

