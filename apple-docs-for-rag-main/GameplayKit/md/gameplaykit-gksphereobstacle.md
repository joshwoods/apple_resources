

- GameplayKit
-  GKSphereObstacle 

Class

# GKSphereObstacle

A spherical impassable volume to be avoided by agents.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class GKSphereObstacle
```

## Overview

To make agents (GKAgent objects) avoid obstacles, create a goal with the init(toAvoid:maxPredictionTime:) method. Agents affected by an avoid-obstacles goal will attempt to move such that their radius never overlaps that of a spherical obstacle.

To learn more about using goals and agents, see Agents, Goals, and Behaviors in GameplayKit Programming Guide.

## Topics

### Creating an Obstacle

init(radius: Float)

Initializes a spherical obstacle with the specified radius.

### Placing an Obstacle

var position: vector_float3

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

class GKCircleObstacle

A circular impassable area to be avoided by agents.

class GKPolygonObstacle

A polygon-shaped impassable area in a 2D game world.

