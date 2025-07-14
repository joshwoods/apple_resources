

- GameplayKit
-  GKGameModelPlayer 

Protocol

# GKGameModelPlayer

Implement this protocol to describe a player in your turn-based game so that a strategist object can plan game moves.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol GKGameModelPlayer : NSObjectProtocol
```

## Overview

You adopt this protocol to describe the gameplay of your turn-based game for use by a GKStrategist object. The strategist uses your player class, along with other custom classes you implement (adopting the GKGameModel and GKGameModelUpdate protocols) to plan moves in your game.

You use your custom class implementing this protocol in several places:

- In the players and activePlayer properties of your game model class, to describe the set of players in your game and indicate which player’s turn it currently is

- In the gameModelUpdates(for:) method of your game model class, to describe the set of moves currently valid for a specified player

- In the isWin(for:), isLoss(for:), and score(for:) method of your game model class, to rate the desirability of that particular state of the game model to a specified player

- When calling the bestMove(for:) or randomMove(for:fromNumberOfBestMoves:) method to find an optimal move, to indicate the player for whom GameplayKit should plan moves

Your class that implements this protocol can also contain properties and methods relevant to the implementation of your game—for example, an identifying color or name.

For more information about describing your gameplay model and using a strategist, see The Minmax Strategist in GameplayKit Programming Guide.

## Topics

### Identifying a Player

var playerId: Int

A number uniquely identifying the player.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Strategists

protocol GKStrategist

A general interface for objects that provide artificial intelligence for use in turn-based (and similar) games.

class GKMinmaxStrategist

An AI that chooses moves in turn-based games using a *deterministic* strategy.

class GKMonteCarloStrategist

An AI that chooses moves in turn-based games using a *probabilistic* strategy.

protocol GKGameModel

Implement this protocol to describe your gameplay model so that a strategist object can plan game moves.

protocol GKGameModelUpdate

Implement this protocol to describe a move in your turn-based game so that a strategist object can plan game moves.

