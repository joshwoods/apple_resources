

- GameplayKit
-  GKCircleObstacle 

Class

# GKCircleObstacle

A circular impassable area to be avoided by agents.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKCircleObstacle
```

## Overview

To make agents (GKAgent objects) avoid obstacles, create a goal with the init(toAvoid:maxPredictionTime:) method. Agents affected by an avoid-obstacles goal will attempt to move such that their radius never overlaps that of a circular obstacle.

To learn more about using goals and agents, see Agents, Goals, and Behaviors in GameplayKit Programming Guide.

## Topics

### Creating an Obstacle

init(radius: Float)

Initializes a circular obstacle with the specified radius.

### Placing an Obstacle

var position: vector_float2

The position of the obstacle.

var radius: Float

The radius of the obstacle.

## Relationships

### Inherits From

- GKObstacle

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Obstacles

class GKObstacle

The abstract base class for objects representing impassable areas in a game world.

class GKSphereObstacle

A spherical impassable volume to be avoided by agents.

class GKPolygonObstacle

A polygon-shaped impassable area in a 2D game world.

