

- GameKit
- GKMatch
-  players 

Instance Property

# players

The players that join the match.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var players: [GKPlayer] { get }
```

## Mentioned in 

Assigning players to teams using rules

## Discussion

This property includes all players except the local player.

## See Also

### Working with other players

var expectedPlayerCount: Int

The remaining number of players invited but not yet connected to the match.

