

- GameplayKit
-  GKPolygonObstacle 

Class

# GKPolygonObstacle

A polygon-shaped impassable area in a 2D game world.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKPolygonObstacle
```

## Overview

Polygon obstacles serve two purposes in GameplayKit: You can use polygon obstacles to construct a navigability graph of your game world (a GKObstacleGraph object) for use in pathfinding. You can also use polygon obstacles to define regions for agents (GKAgent objects) to avoid, using the GKGoal method init(toAvoid:maxPredictionTime:).

To easily create obstacles for use with a SpriteKit game, create and arrange a set of nodes that define the non-navigable regions of your game world. You can create such nodes programmatically, or use the SpriteKit Scene Editor in Xcode. If you’re already using nodes with physics bodies to keep sprites from entering those regions, you can reuse those nodes. Then, use the obstacles(fromNodeBounds:), obstacles(fromSpriteTextures:accuracy:), or obstacles(fromNodePhysicsBodies:) method to generate a set of GKPolygonObstacle objects.

To learn more about both ways of using polygon obstacles, see Pathfinding and Agents, Goals, and Behaviors in GameplayKit Programming Guide.

## Topics

### Inspecting Vertices

var vertexCount: Int

The number of vertices that define the polygon-shaped area of the obstacle.

func vertex(at: Int) -> vector_float2

Returns the point coordinates of the specified vertex.

### Initializers

convenience init(points: [SIMD2&lt;Float>])

## Relationships

### Inherits From

- GKObstacle

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Obstacles

class GKObstacle

The abstract base class for objects representing impassable areas in a game world.

class GKCircleObstacle

A circular impassable area to be avoided by agents.

class GKSphereObstacle

A spherical impassable volume to be avoided by agents.

