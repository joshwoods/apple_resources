

- GameplayKit
- GKGameModel
-  Game Model Score Limits 

API Collection

# Game Model Score Limits

Limits to values returned by the score(for:) method.

## Overview

When you evaluate the state of a game model in the score(for:) method, the GKMinmaxStrategist class weights the resulting value by search depth and performs other calculations in its process of selecting an optimal move. To prevent overflow errors in such calculations, keep scores within the range of GKGameModelMinScore to GKGameModelMaxScore, inclusive.

## Topics

### Constants

let GKGameModelMaxScore: Int

The maximum return value allowed for the score(for:) method.

let GKGameModelMinScore: Int

The minimum return value allowed for the score(for:) method.

