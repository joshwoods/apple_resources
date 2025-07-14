

- GameplayKit
-  GKMonteCarloStrategist 

Class

# GKMonteCarloStrategist

An AI that chooses moves in turn-based games using a *probabilistic* strategy.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class GKMonteCarloStrategist
```

## Overview

To use this strategy, you indicate whether a possible states of your game model represents a win, and the strategist randomly searches possible game model states in order to find moves that will likely result in winning the game. You provide information about your game model to the strategist by implementing the GKGameModel, GKGameModelPlayer, and GKGameModelUpdate protocols in your custom classes, then use the strategist’s methods to find optimal moves.

### Choosing a Strategist

The Monte Carlo strategist is one of several strategist classes that GameplayKit provides. The key advantage of the GKMonteCarloStrategist class is performance. By using random sampling to make educated guesses about which sequences of moves to simulate, this strategy can arrive at a decision quickly even for games with large and complex state spaces. The cost of this strategy is strength of gameplay: because the strategist randomly samples possible moves, it may miss the best moves. Additionally, this strategy doesn’t need a scoring method to rate each game model state—instead, your game model class needs to implement only the isWin(for:) method.

See the GKStrategist protocol for alternate strategies, as well as the methods and properties supported by all strategist classes.

### Using a Monte Carlo Strategist

Using the Monte Carlo strategist in a game requires the following steps:

1.  Create classes describing your gameplay model, adopting the GKGameModel, GKGameModelPlayer, and GKGameModelUpdate protocols.

2.  Create a GKMonteCarloStrategist instance and configure its properties budget, explorationParameter, and randomSource to determine its gameplay behavior.

3.  Point the strategist’s gameModel property at the instance of your game model class (that is, your class that implements the GKGameModel protocol) representing the current state of the game in play.

4.  Use the bestMoveForActivePlayer() method to select the best possible move for the current player. This method returns a move object (that is, an instance of the custom class you create to adopt the GKGameModelUpdate protocol).

5.  Examine the move object to make use of the move selected by the strategist. You created this instance in the gameModelUpdates(for:) method of your game model class to describe a possible move in your game, so examining the object gives you the information needed to perform that move.

For more information about describing your gameplay model and using strategists, see The Minmax Strategist in GameplayKit Programming Guide.

## Topics

### Configuring a Strategist

var budget: Int

The maximum number of game model states the strategist will examine when searching for a move.

var explorationParameter: Int

A value that influences whether the strategist searches more broadly or more deeply for winning game model states.

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

class GKMinmaxStrategist

An AI that chooses moves in turn-based games using a *deterministic* strategy.

protocol GKGameModel

Implement this protocol to describe your gameplay model so that a strategist object can plan game moves.

protocol GKGameModelPlayer

Implement this protocol to describe a player in your turn-based game so that a strategist object can plan game moves.

protocol GKGameModelUpdate

Implement this protocol to describe a move in your turn-based game so that a strategist object can plan game moves.

