

- GameplayKit
- GKGameModel
-  apply(\_:) 

Instance Method

# apply(\_:)

Updates the internal state of the game model to reflect the specified changes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func apply(_ gameModelUpdate: any GKGameModelUpdate)
```

**Required**

## Parameters 

`gameModelUpdate`  

An instance of your custom class that implements the GKGameModelUpdate protocol, describing a move to be made in your game.

## Discussion

Your implementation of the GKGameModelUpdate protocol, or *move class*, should add properties or methods that describe a move in terms of your game. In this method, you examine that information and perform the corresponding changes to your game model’s internal state. GameplayKit calls this method to speculate about possible future moves and their effects, using a copy of the active game board.

For example, a move class for a chess game would identify the piece to be moved and the space to which the piece will move. Your apply(_:) method would update its model of the game board to reflect the new location of that piece and perform any actions that result from the move, such as capturing other pieces.

GameplayKit assumes that calling this method performs a move on behalf of the player identified by the activePlayer property.

Note

By default, a GameplayKit strategist explores possible moves by copying the current game model, then calling this method to test the effect of a move. Copying a game model (see the setGameModel(_:) method) repeatedly can increase the time it takes for a strategist to evaluate moves. If you also implement the unapplyGameModelUpdate(_:) method to undo moves, the strategist can evaluate multiple moves without copying the game model, possibly increasing performance.

## See Also

### Modifying a Game Model

func unapplyGameModelUpdate(any GKGameModelUpdate)

Updates the internal state of the game model to remove the effect of the specified changes.

func setGameModel(any GKGameModel)

Sets the game model’s internal state to that of the specified game model.

**Required**

