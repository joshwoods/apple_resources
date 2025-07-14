

- GameplayKit
- GKGameModel
-  isLoss(for:) 

Instance Method

# isLoss(for:)

Returns a Boolean value indicating whether the specified player has lost the game.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
optional func isLoss(for player: any GKGameModelPlayer) -> Bool
```

## Parameters 

`player`  

An instance of your game’s player class (a custom class implementing the GKGameModelPlayer protocol) representing the player evaluating the game model.

## Return Value

true if this game model represents a losing state for the specified player; false if the game has been won or has not yet concluded.

## Discussion

If the game has been won or lost, a strategist evaluating the game model can avoid evaluating further moves in the game and can therefore plan a successful move more efficiently.

For some games, merely identifying winning and losing states of the game model and using a sufficiently large maxLookAheadDepth value is enough for a strategist to play the game well. However, you can improve both the game performance and the runtime efficiency of move planning by also implementing the score(for:) method to distinguish the relative desirability of non-game-ending states.

Note

This method is optional; however, your game model class must implement at least one of the score(for:), isLoss(for:), and isWin(for:) methods.

## See Also

### Evaluating a Game Model

func gameModelUpdates(for: any GKGameModelPlayer) -> [any GKGameModelUpdate]?

Returns the set of moves available to the specified player.

**Required**

func score(for: any GKGameModelPlayer) -> Int

Returns a number rating the desirability of the game model’s current state from the perspective of the specified player.

func isWin(for: any GKGameModelPlayer) -> Bool

Returns a Boolean value indicating whether the current state of the game model reflects a win for the specified player.

