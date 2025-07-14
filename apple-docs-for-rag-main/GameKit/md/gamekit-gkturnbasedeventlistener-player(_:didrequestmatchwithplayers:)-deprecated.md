

- GameKit
- GKTurnBasedEventListener
-  player(\_:didRequestMatchWithPlayers:) Deprecated

Instance Method

# player(\_:didRequestMatchWithPlayers:)

Handles when the player uses Game Center to start a match with other players.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
optional func player(
    _ player: GKPlayer,
    didRequestMatchWithPlayers playerIDsToInvite: [String]
)
```

Deprecated

Use the player(_:didRequestMatchWithOtherPlayers:) method instead.

## Parameters 

`player`  

The player who receives this turn-based event. .

`playerIDsToInvite`  

The identifiers for the players to invite in the view controller interface.

## Discussion

Implement this method to present a GKTurnBasedMatchmakerViewController configured with the players to invite specified by the `playerIDsToInvite` parameter.

## See Also

### Handling Match-Related Events

func player(GKPlayer, receivedTurnEventFor: GKTurnBasedMatch, didBecomeActive: Bool)

Handles turn-based match events, such as accepting invitations, passing turns, and saving match data.

func player(GKPlayer, didRequestMatchWithOtherPlayers: [GKPlayer])

Handles when the player uses Game Center to start a match with other players.

func player(GKPlayer, matchEnded: GKTurnBasedMatch)

Handles when the match ends.

func player(GKPlayer, wantsToQuitMatch: GKTurnBasedMatch)

Handles when the current participant wants to quit a match.

