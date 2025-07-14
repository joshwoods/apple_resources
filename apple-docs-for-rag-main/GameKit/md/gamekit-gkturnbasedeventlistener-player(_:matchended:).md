

- GameKit
- GKTurnBasedEventListener
-  player(\_:matchEnded:) 

Instance Method

# player(\_:matchEnded:)

Handles when the match ends.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
optional func player(
    _ player: GKPlayer,
    matchEnded match: GKTurnBasedMatch
)
```

## Parameters 

`player`  

The player who receives this turn-based event.

`match`  

The match that ends.

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

Implement this method to stop gameplay, notify the player that the match is over, and show the participant outcomes.

## See Also

### Handling Match-Related Events

func player(GKPlayer, receivedTurnEventFor: GKTurnBasedMatch, didBecomeActive: Bool)

Handles turn-based match events, such as accepting invitations, passing turns, and saving match data.

func player(GKPlayer, didRequestMatchWithOtherPlayers: [GKPlayer])

Handles when the player uses Game Center to start a match with other players.

func player(GKPlayer, wantsToQuitMatch: GKTurnBasedMatch)

Handles when the current participant wants to quit a match.

func player(GKPlayer, didRequestMatchWithPlayers: [String])

Handles when the player uses Game Center to start a match with other players.

Deprecated

