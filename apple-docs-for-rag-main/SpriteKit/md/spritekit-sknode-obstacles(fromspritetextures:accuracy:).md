

- SpriteKit
- SKNode
-  obstacles(fromSpriteTextures:accuracy:) 

Type Method

# obstacles(fromSpriteTextures:accuracy:)

Turns each node into an obstacle by changing the node’s texture into a physics shape and converting it into the scene’s coordinate system.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
class func obstacles(
    fromSpriteTextures sprites: [SKNode],
    accuracy: Float
) -> [GKPolygonObstacle]
```

## Parameters 

`sprites`  

An array of SKNode objects.

`accuracy`  

A floating point value between `0.001` and `1.0`, inclusive. Higher values create a more precise (but more complex) representation of the obstacle.

## Return Value

An array of GKPolygonObstacle objects.

## Discussion

Use the array of obstacles to create an obstacle graph (GKObstacleGraph) in GameplayKit. See GameplayKit and GameplayKit Programming Guide.

## See Also

### Adding GameplayKit Behaviors

var entity: GKEntity?

The GameplayKit entity this node represents.

class func obstacles(fromNodeBounds: [SKNode]) -> [GKPolygonObstacle]

Converts each node into an obstacle by transforming its bounds into the scene’s coordinate system.

class func obstacles(fromNodePhysicsBodies: [SKNode]) -> [GKPolygonObstacle]

Converts each node into an obstacle by transforming the node’s physics body shape into the scene’s coordinate system.

