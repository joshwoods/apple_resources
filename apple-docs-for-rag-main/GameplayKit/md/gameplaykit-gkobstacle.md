

- GameplayKit
-  GKObstacle 

Class

# GKObstacle

The abstract base class for objects representing impassable areas in a game world.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKObstacle
```

## Overview

You do not use this class directly; instead, create instances of its concrete subclasses GKCircleObstacle, GKSphereObstacle, and GKPolygonObstacle. To make agents (GKAgent objects) avoid obstacles, create a goal with the goalToAvoidObstacles:timeBeforeCollisionToAvoid: method.

To learn more about using goals and agents, see Agents, Goals, and Behaviors in GameplayKit Programming Guide.

For more information, see GameplayKit Programming Guide.

## Relationships

### Inherits From

- NSObject

### Inherited By

- GKCircleObstacle
- GKPolygonObstacle
- GKSphereObstacle

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Obstacles

class GKCircleObstacle

A circular impassable area to be avoided by agents.

class GKSphereObstacle

A spherical impassable volume to be avoided by agents.

class GKPolygonObstacle

A polygon-shaped impassable area in a 2D game world.

