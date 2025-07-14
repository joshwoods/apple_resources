

- GameplayKit
- GKStrategist
-  bestMoveForActivePlayer() 

Instance Method

# bestMoveForActivePlayer()

Computes and returns the best possible move for the current player.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func bestMoveForActivePlayer() -> (any GKGameModelUpdate)?
```

**Required**

## Return Value

An object describing the move found by the strategist.

## Discussion

This method looks ahead at the possible moves for the current player (as specified by the activePlayer of the strategist’s game model), as well as possible future moves by other players on subsequent turns, and examines the state of the game model resulting from each possible move. Your game model class rates the desirability of its current state, allowing the strategist to find the sequence of future moves that results in the best outcome for the current player and to return the first move in that sequence.

The object returned is an instance of your custom class implementing the GKGameModelUpdate protocol. Your game model’s gameModelUpdates(for:) method creates this object, describing in your game’s terms a possible move. For example, the game model update class for a Tic-Tac-Toe game would add properties indicating which position an X or O marker is to be placed in. To make use of the strategist’s selection, examine this information you added to the object when creating it. You can implement a computer-controlled player by performing the selected move, or provide hints to a human player by indicating the selected move in your game’s user interface.

Important

For the GKMonteCarloStrategist class, or a custom class that requires randomization, you must set the the randomSource property before calling the bestMoveForActivePlayer() method. (For the GKMinmaxStrategist class, or custom classes with deterministic strategies, a random source is optional.)

This method returns `nil` if the current player is invalid or has no available moves.

