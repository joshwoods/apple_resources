

- GameplayKit
- GKMonteCarloStrategist
-  budget 

Instance Property

# budget

The maximum number of game model states the strategist will examine when searching for a move.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var budget: Int { get set }
```

## Discussion

When you call the bestMoveForActivePlayer() method, the Monte Carlo strategist randomly chooses between the available moves for the current player (see the gameModelUpdates(for:) method of your game model class), then randomly chooses a subsequent move, and so on, until it reaches a state in which the game is either won or lost. Then it returns to the original game state and repeats that process, accumulating information about which sequences of moves are more or less likely to result in a win. When the strategist examines a number of moves equal to the value of its budget property, it stops, and returns the move it currently rates as “best”.

The default value of 15 is well-suited for situations where the strategist will find at least one possible win after examining 15 moves. (Such situations might occur in games where only a few moves are possible on each turn, or when the end of a game is only a few moves away from the current state.) Higher values allow the strategist to accumulate more information about which moves are most likely to result in a win, but increase the amount of time required to choose a move.

For more information, see GameplayKit Programming Guide.

## See Also

### Configuring a Strategist

var explorationParameter: Int

A value that influences whether the strategist searches more broadly or more deeply for winning game model states.

