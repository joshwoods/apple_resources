

- GameKit
- GKMatchRequest
-  recipients 

Instance Property

# recipients

The players to invite to the match.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var recipients: [GKPlayer]? { get set }
```

## Mentioned in 

Finding multiple players for a game

Finding players using matchmaking rules

Finding players with similar skill levels

## Discussion

If this property is non-`nil`, GameKit invites the specified players. GameKit doesn’t use automatch to fill player slots, and ignores the maxPlayers and minPlayers properties. The default value is `nil`.

## See Also

### Inviting players

var inviteMessage: String?

The message sent to other players when the local player invites them to join a match.

var recipientResponseHandler: ((GKPlayer, GKInviteRecipientResponse) -> Void)?

A method that handles when a player responds to an invitation to join a match.

enum GKInviteRecipientResponse

A player’s response to an invitation to join a match.

