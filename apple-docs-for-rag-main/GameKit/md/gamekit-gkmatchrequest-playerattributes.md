

- GameKit
- GKMatchRequest
-  playerAttributes 

Instance Property

# playerAttributes

A mask that specifies the role that the local player would like to play in the game.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var playerAttributes: UInt32 { get set }
```

## Mentioned in 

Finding players using matchmaking rules

## Discussion

If the value of this property is `0xFFFFFFFF` (the default), GameKit ignores this property. If the value is nonzero, GameKit uses the value as a mask that restricts the role of the player in the match. GameKit finds new players for the game so that the bitwise OR of all the player’s masks equals `0xFFFFFFFF`.

## See Also

### Matching specific players

var playerGroup: Int

A number identifying a subset of players invited to join a match.

