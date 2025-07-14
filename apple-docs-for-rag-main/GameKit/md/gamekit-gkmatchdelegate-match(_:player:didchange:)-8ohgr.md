

- GameKit
- GKMatchDelegate
-  match(\_:player:didChange:) 

Instance Method

# match(\_:player:didChange:)

Handles when players connect or disconnect from a match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
optional func match(
    _ match: GKMatch,
    player: GKPlayer,
    didChange state: GKPlayerConnectionState
)
```

## Parameters 

`match`  

The match joined by the player.

`player`  

The player whose state changed.

`state`  

The state of the player in the match.

## Mentioned in 

Finding multiple players for a game

Exchanging data between players in real-time games

## Discussion

If the match’s expectedPlayerCount property is `0` when GameKit invokes this method, you can start the game. If two or more players join the match, you can begin data and voice communication.

## See Also

### Receiving State Notifications About Other Players

enum GKPlayerConnectionState

The possible states of a connection to a match.

