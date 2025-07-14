

- GameKit
- GKInviteEventListener
-  player(\_:didAccept:) 

Instance Method

# player(\_:didAccept:)

Handles the event when the local player accepts an invitation from another player.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func player(
    _ player: GKPlayer,
    didAccept invite: GKInvite
)
```

## Parameters 

`player`  

The local player who accepts the invitation.

`invite`  

The invitation that the local player accepts.

## Mentioned in 

Finding multiple players for a game

## Discussion

This method presents the matchmaker view controller in the invitation state so that the local player can see other players in the match accept their invitations.

## See Also

### Related Documentation

Finding multiple players for a game

Discover and invite other players to participate in a real-time game.

### Starting a New Match

func player(GKPlayer, didRequestMatchWithRecipients: [GKPlayer])

Handles the event when the local player sends other players an invitation to join a match.

func player(GKPlayer, didRequestMatchWithPlayers: [String])

Handles the event when the local player sends other players an invitation to join a match.

Deprecated

