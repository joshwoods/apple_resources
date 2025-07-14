

- GameplayKit
-  GKStrategist 

Protocol

# GKStrategist

A general interface for objects that provide artificial intelligence for use in turn-based (and similar) games.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol GKStrategist : NSObjectProtocol
```

## Overview

GameplayKit provides two strategist classes, and you can also use this protocol to implement your own. You provide information about your game model to a strategist by implementing the GKGameModel, GKGameModelPlayer, and GKGameModelUpdate protocols in your custom classes, then use the strategist’s methods to find optimal moves.

### Choosing a Strategist

GameplayKit provides two strategist classes:

- The GKMinmaxStrategist class uses a numeric score for each possible game model state, and performs an exhaustive tree search to find moves that maximize the player’s score while minimizing opponent scores. This strategy can result in optimal gameplay, but requires a scoring method for game models and has a performance cost that increases greatly with game complexity.

- The GKMonteCarloStrategist class performs a randomized, probabilistic search for winning end states. This strategy doesn’t always choose the *best* possible move, but is likely to choose *good* moves, and has a low performance cost even for very complex games. In addition, the Monte Carlo strategy is concerned only with whether a game model state represents a win, so you don’t need to implement a scoring method.

### Using a Strategist

Using a strategist in a game requires the following steps:

1.  Create classes describing your gameplay model, adopting the GKGameModel, GKGameModelPlayer, and GKGameModelUpdate protocols.

2.  Choose a strategist class (one that adopts the GKStrategist protocol), create an instance of that class, and configure its properties to determine its gameplay behavior.

3.  Point the strategist’s gameModel property at the instance of your game model class representing the current state of the game in play.

4.  Use the bestMoveForActivePlayer() method to select the best possible move for the current player. This method returns a move object (that is, an instance of the custom class you create to adopt the GKGameModelUpdate protocol).

5.  Examine the move object to make use of the move selected by the strategist. You created this instance in the gameModelUpdates(for:) method of your game model class to describe a possible move in your game, so examining the object gives you the information needed to perform that move.

For more information about describing your gameplay model and using strategists, see The Minmax Strategist in GameplayKit Programming Guide.

## Topics

### Specifying the Game Model

var gameModel: (any GKGameModel)?

The model representing the current state of the game.

**Required**

### Configuring a Strategist

var randomSource: (any GKRandom)?

A randomizer object to be used when the strategist randomly selects a move.

**Required**

### Planning Game Moves

func bestMoveForActivePlayer() -> (any GKGameModelUpdate)?

Computes and returns the best possible move for the current player.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- GKMinmaxStrategist
- GKMonteCarloStrategist

## See Also

### Strategists

class GKMinmaxStrategist

An AI that chooses moves in turn-based games using a *deterministic* strategy.

class GKMonteCarloStrategist

An AI that chooses moves in turn-based games using a *probabilistic* strategy.

protocol GKGameModel

Implement this protocol to describe your gameplay model so that a strategist object can plan game moves.

protocol GKGameModelPlayer

Implement this protocol to describe a player in your turn-based game so that a strategist object can plan game moves.

protocol GKGameModelUpdate

Implement this protocol to describe a move in your turn-based game so that a strategist object can plan game moves.

