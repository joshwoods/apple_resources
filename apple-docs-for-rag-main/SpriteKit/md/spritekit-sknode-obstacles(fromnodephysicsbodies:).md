

- SpriteKit
- SKNode
-  obstacles(fromNodePhysicsBodies:) 

Type Method

# obstacles(fromNodePhysicsBodies:)

Converts each node into an obstacle by transforming the node’s physics body shape into the scene’s coordinate system.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
class func obstacles(fromNodePhysicsBodies nodes: [SKNode]) -> [GKPolygonObstacle]
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

class func obstacles(fromNodeBounds: [SKNode]) -> [GKPolygonObstacle]

Converts each node into an obstacle by transforming its bounds into the scene’s coordinate system.

class func obstacles(fromSpriteTextures: [SKNode], accuracy: Float) -> [GKPolygonObstacle]

Turns each node into an obstacle by changing the node’s texture into a physics shape and converting it into the scene’s coordinate system.

