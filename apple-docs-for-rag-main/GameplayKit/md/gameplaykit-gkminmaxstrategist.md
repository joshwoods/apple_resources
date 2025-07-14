

- GameplayKit
-  GKMinmaxStrategist 

Class

# GKMinmaxStrategist

An AI that chooses moves in turn-based games using a *deterministic* strategy.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKMinmaxStrategist
```

## Overview

To use this strategy, you provide scores that rate possible states of your game model for their desirability to a player, and the strategist exhaustively searches all possible game model states in order to make choices that maximize the rating for its own moves and minimize the rating for an opponent’s moves. You provide information about your game model to the strategist by implementing the GKGameModel, GKGameModelPlayer, and GKGameModelUpdate protocols in your custom classes, and then use the strategist’s methods to find optimal moves.

### Choosing a Strategist

GameplayKit provides multiple strategist classes. The advantage of the GKMinmaxStrategist class is its deterministic, exhaustive strategy: If allowed, the minmax strategist searches the entire space of possible moves and the game states they lead to, so it can find the best possible move at any time. The cost of this strategy is performance: searching every possible game state takes time, especially for complex games where many moves are possible at any given time. Additionally, this strategy requires that your game model implement the score(for:) method to rate the desirability of each game state.

See the GKStrategist protocol for alternate strategies, as well as the methods and properties supported by all strategist classes.

### Using a Minmax Strategist

Using the minmax strategist in a game requires the following steps:

1.  Create classes describing your gameplay model, adopting the GKGameModel, GKGameModelPlayer, and GKGameModelUpdate protocols.

2.  Create GKMinmaxStrategist instance and configure its properties maxLookAheadDepth and randomSource to determine its gameplay behavior.

3.  Point the minmax strategist’s gameModel property at the instance of your game model class (that is, your class that implements the GKGameModel protocol) representing the current state of the game in play.

4.  Use the bestMoveForActivePlayer() method to select the best possible move for the current player. This method returns a move object (that is, an instance of the custom class you create to adopt the GKGameModelUpdate protocol).

5.  Examine the move object to make use of the move selected by the strategist. You created this instance in the gameModelUpdates(for:) method of your game model class to describe a possible move in your game, so examining the object gives you the information needed to perform that move.

For more information about describing your gameplay model and using strategists, see The Minmax Strategist in GameplayKit Programming Guide.

## Topics

### Configuring a Strategist

var maxLookAheadDepth: Int

The number of future turns for the strategist to consider when planning moves.

### Planning Game Moves

func bestMove(for: any GKGameModelPlayer) -> (any GKGameModelUpdate)?

Computes and returns the best possible move for the specified player.

func randomMove(for: any GKGameModelPlayer, fromNumberOfBestMoves: Int) -> (any GKGameModelUpdate)?

Computes several of the best possible moves for the specified player, and returns a move randomly selected from among them.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GKStrategist
- Hashable
- NSObjectProtocol

## See Also

### Strategists

protocol GKStrategist

A general interface for objects that provide artificial intelligence for use in turn-based (and similar) games.

class GKMonteCarloStrategist

An AI that chooses moves in turn-based games using a *probabilistic* strategy.

protocol GKGameModel

Implement this protocol to describe your gameplay model so that a strategist object can plan game moves.

protocol GKGameModelPlayer

Implement this protocol to describe a player in your turn-based game so that a strategist object can plan game moves.

protocol GKGameModelUpdate

Implement this protocol to describe a move in your turn-based game so that a strategist object can plan game moves.

