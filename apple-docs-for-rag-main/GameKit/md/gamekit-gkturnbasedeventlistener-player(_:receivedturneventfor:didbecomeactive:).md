

- GameKit
- GKTurnBasedEventListener
-  player(\_:receivedTurnEventFor:didBecomeActive:) 

Instance Method

# player(\_:receivedTurnEventFor:didBecomeActive:)

Handles turn-based match events, such as accepting invitations, passing turns, and saving match data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
optional func player(
    _ player: GKPlayer,
    receivedTurnEventFor match: GKTurnBasedMatch,
    didBecomeActive: Bool
)
```

## Parameters 

`player`  

The player who receives this turn-based event.

`match`  

The match related to this turn-based event.

`didBecomeActive`  

true if the system launches the game to deliver the turn-based event; otherwise, false.

## Mentioned in 

Starting turn-based matches and passing turns between players

Sending messages to players in turn-based games

Exchanging data between players in turn-based games

## Discussion

GameKit invokes this method when these turn-based events occur:

- GameKit passes the turn to the player.

- The player accepts an invitation from another participant.

- The timeout for the player to take their turn is about to expire.

- A participant saves match data to Game Center.

- Another participant sends a reminder to the player.

- The player opens an existing or completed match.

- The player forfeits a match.

## See Also

### Handling Match-Related Events

func player(GKPlayer, didRequestMatchWithOtherPlayers: [GKPlayer])

Handles when the player uses Game Center to start a match with other players.

func player(GKPlayer, matchEnded: GKTurnBasedMatch)

Handles when the match ends.

func player(GKPlayer, wantsToQuitMatch: GKTurnBasedMatch)

Handles when the current participant wants to quit a match.

func player(GKPlayer, didRequestMatchWithPlayers: [String])

Handles when the player uses Game Center to start a match with other players.

Deprecated

