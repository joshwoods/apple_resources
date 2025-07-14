

- GameplayKit
- GKGameModel
-  players 

Instance Property

# players

The players currently in the game.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var players: [any GKGameModelPlayer]? { get }
```

**Required**

## Discussion

This array should contain instances of your player class (a custom class implementing the GKGameModelPlayer protocol) representing the players in the game. When you use the GKMinmaxStrategist class to find an optimal move for a specific player, GameplayKit uses this array to rate the moves of that player’s opponent(s).

For more information, see GameplayKit Programming Guide.

## See Also

### Keeping Track of Players

var activePlayer: (any GKGameModelPlayer)?

The player whose turn it currently is in the game.

**Required**

