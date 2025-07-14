

- SpriteKit
- SKNode
-  obstacles(fromNodeBounds:) 

Type Method

# obstacles(fromNodeBounds:)

Converts each node into an obstacle by transforming its bounds into the scene’s coordinate system.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
class func obstacles(fromNodeBounds nodes: [SKNode]) -> [GKPolygonObstacle]
```

## Parameters 

`nodes`  

An array of SKNode objects.

## Return Value

An array of GKPolygonObstacle objects.

## Discussion

Use the array of obstacles to create an obstacle graph (GKObstacleGraph) in GameplayKit. See GameplayKit and GameplayKit Programming Guide.

## See Also

### Adding GameplayKit Behaviors

var entity: GKEntity?

The GameplayKit entity this node represents.

class func obstacles(fromNodePhysicsBodies: [SKNode]) -> [GKPolygonObstacle]

Converts each node into an obstacle by transforming the node’s physics body shape into the scene’s coordinate system.

class func obstacles(fromSpriteTextures: [SKNode], accuracy: Float) -> [GKPolygonObstacle]

Turns each node into an obstacle by changing the node’s texture into a physics shape and converting it into the scene’s coordinate system.

