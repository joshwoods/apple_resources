

- GameKit
- GKMatchRequest
-  playerGroup 

Instance Property

# playerGroup

A number identifying a subset of players invited to join a match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var playerGroup: Int { get set }
```

## Mentioned in 

Finding players using matchmaking rules

Creating matchmaking rules for backward compatibility

## Discussion

Game Center only finds players whose `GKMatchRequest` objects share the same `playerGroup` value. For example, use the `playerGroup` property to create matches based on skill level, game modes, or other common interests. The default value of this property is `1`.

## See Also

### Matching specific players

var playerAttributes: UInt32

A mask that specifies the role that the local player would like to play in the game.

