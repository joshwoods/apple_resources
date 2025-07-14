

- SpriteKit
- SKNode
-  entity 

Instance Property

# entity

The GameplayKit entity this node represents.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
weak var entity: GKEntity? { get set }
```

## Discussion

The Entity-Component architecture in the GameplayKit framework is a way to more easily manage complex object graphs in your game. For more information on this architecture, read Entities and Components in GameplayKit Programming Guide.

When you add entities (and their components) to a scene in the Xcode SpriteKit Scene Editor, Xcode automatically archive those entities alongside the SpriteKit scene content. Use the GKScene class to load the SpriteKit scene with its associated GameplayKit objects. Each entity associated with a SpriteKit node has a GKSKNodeComponent object that manages the relationship between the node and the GKEntity object it represents.

## See Also

### Adding GameplayKit Behaviors

class func obstacles(fromNodeBounds: [SKNode]) -> [GKPolygonObstacle]

Converts each node into an obstacle by transforming its bounds into the scene’s coordinate system.

class func obstacles(fromNodePhysicsBodies: [SKNode]) -> [GKPolygonObstacle]

Converts each node into an obstacle by transforming the node’s physics body shape into the scene’s coordinate system.

class func obstacles(fromSpriteTextures: [SKNode], accuracy: Float) -> [GKPolygonObstacle]

Turns each node into an obstacle by changing the node’s texture into a physics shape and converting it into the scene’s coordinate system.

