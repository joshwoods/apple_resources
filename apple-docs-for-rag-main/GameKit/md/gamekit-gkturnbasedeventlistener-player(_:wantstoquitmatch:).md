

- GameKit
- GKTurnBasedEventListener
-  player(\_:wantsToQuitMatch:) 

Instance Method

# player(\_:wantsToQuitMatch:)

Handles when the current participant wants to quit a match.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
optional func player(
    _ player: GKPlayer,
    wantsToQuitMatch match: GKTurnBasedMatch
)
```

## Parameters 

`player`  

The player who receives this turn-based event.

`match`  

The match that the current participant wants to quit.

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

Implement this method to forfeit the match by passing the turn to the next participant using the participantQuitInTurn(with:nextParticipants:turnTimeout:match:completionHandler:) method.

## See Also

### Handling Match-Related Events

func player(GKPlayer, receivedTurnEventFor: GKTurnBasedMatch, didBecomeActive: Bool)

Handles turn-based match events, such as accepting invitations, passing turns, and saving match data.

func player(GKPlayer, didRequestMatchWithOtherPlayers: [GKPlayer])

Handles when the player uses Game Center to start a match with other players.

func player(GKPlayer, matchEnded: GKTurnBasedMatch)

Handles when the match ends.

func player(GKPlayer, didRequestMatchWithPlayers: [String])

Handles when the player uses Game Center to start a match with other players.

Deprecated

