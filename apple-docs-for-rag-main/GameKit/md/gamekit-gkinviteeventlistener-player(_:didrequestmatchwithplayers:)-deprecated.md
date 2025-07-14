

- GameKit
- GKInviteEventListener
-  player(\_:didRequestMatchWithPlayers:) Deprecated

Instance Method

# player(\_:didRequestMatchWithPlayers:)

Handles the event when the local player sends other players an invitation to join a match.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func player(
    _ player: GKPlayer,
    didRequestMatchWithPlayers playerIDsToInvite: [String]
)
```

Deprecated

Use the player(_:didRequestMatchWithRecipients:) method instead.

## Parameters 

`player`  

The local player who sends the invitation.

`playerIDsToInvite`  

The identifiers for the players who receive invitations to join the match.

## Discussion

When you call this method, GameKit launches the game and starts the matchmaking process.

## See Also

### Starting a New Match

func player(GKPlayer, didAccept: GKInvite)

Handles the event when the local player accepts an invitation from another player.

func player(GKPlayer, didRequestMatchWithRecipients: [GKPlayer])

Handles the event when the local player sends other players an invitation to join a match.

