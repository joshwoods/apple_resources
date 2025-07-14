

- GameKit
- GKMatchRequest
-  inviteMessage 

Instance Property

# inviteMessage

The message sent to other players when the local player invites them to join a match.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var inviteMessage: String? { get set }
```

## See Also

### Inviting players

var recipients: [GKPlayer]?

The players to invite to the match.

var recipientResponseHandler: ((GKPlayer, GKInviteRecipientResponse) -> Void)?

A method that handles when a player responds to an invitation to join a match.

enum GKInviteRecipientResponse

A player’s response to an invitation to join a match.

