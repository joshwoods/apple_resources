

- GameKit
- GKTurnBasedEventListener
-  player(\_:didRequestMatchWithOtherPlayers:) 

Instance Method

# player(\_:didRequestMatchWithOtherPlayers:)

Handles when the player uses Game Center to start a match with other players.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func player(
    _ player: GKPlayer,
    didRequestMatchWithOtherPlayers playersToInvite: [GKPlayer]
)
```

## Parameters 

`player`  

The player who receives this turn-based event.

`playersToInvite`  

The players to invite in the view controller interface.

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

Implement this method to present a turn-based matchmaker interface configured with the players to invite:

1.  Create a GKMatchRequest object.

2.  Set the match request’s recipients property to `playersToInvite`.

3.  Create a GKTurnBasedMatchmakerViewController with the match request object.

4.  Present the turn-based matchmaker view controller.

## See Also

### Handling Match-Related Events

func player(GKPlayer, receivedTurnEventFor: GKTurnBasedMatch, didBecomeActive: Bool)

Handles turn-based match events, such as accepting invitations, passing turns, and saving match data.

func player(GKPlayer, matchEnded: GKTurnBasedMatch)

Handles when the match ends.

func player(GKPlayer, wantsToQuitMatch: GKTurnBasedMatch)

Handles when the current participant wants to quit a match.

func player(GKPlayer, didRequestMatchWithPlayers: [String])

Handles when the player uses Game Center to start a match with other players.

Deprecated

