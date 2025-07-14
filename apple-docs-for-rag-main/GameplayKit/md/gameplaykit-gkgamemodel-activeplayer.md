

- GameplayKit
- GKGameModel
-  activePlayer 

Instance Property

# activePlayer

The player whose turn it currently is in the game.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var activePlayer: (any GKGameModelPlayer)? { get }
```

**Required**

## Discussion

This player is responsible for the next move. GameplayKit assumes that the next call to the apply(_:) method will perform a move on behalf of this player.

## See Also

### Keeping Track of Players

var players: [any GKGameModelPlayer]?

The players currently in the game.

**Required**

