

- GameKit
- GKMatch
-  expectedPlayerCount 

Instance Property

# expectedPlayerCount

The remaining number of players invited but not yet connected to the match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
var expectedPlayerCount: Int { get }
```

## Mentioned in 

Exchanging data between players in real-time games

## Discussion

GameKit decrements the value of this property when a player connects to the match. When the value reaches `0`, all expected players joined, and the game can begin.

## See Also

### Working with other players

var players: [GKPlayer]

The players that join the match.

