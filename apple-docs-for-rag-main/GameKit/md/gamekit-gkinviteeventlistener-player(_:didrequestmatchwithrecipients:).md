

- GameKit
- GKInviteEventListener
-  player(\_:didRequestMatchWithRecipients:) 

Instance Method

# player(\_:didRequestMatchWithRecipients:)

Handles the event when the local player sends other players an invitation to join a match.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func player(
    _ player: GKPlayer,
    didRequestMatchWithRecipients recipientPlayers: [GKPlayer]
)
```

## Parameters 

`player`  

The local player who sends the invitation.

`recipientPlayers`  

The players who receive invitations to join the match.

## Discussion

When GameKit calls this method, Game Center starts the matchmaking process.

## See Also

### Starting a New Match

func player(GKPlayer, didAccept: GKInvite)

Handles the event when the local player accepts an invitation from another player.

func player(GKPlayer, didRequestMatchWithPlayers: [String])

Handles the event when the local player sends other players an invitation to join a match.

Deprecated

