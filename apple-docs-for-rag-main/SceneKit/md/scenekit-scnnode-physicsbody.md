

- SceneKit
- SCNNode
-  physicsBody 

Instance Property

# physicsBody

The physics body associated with the node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var physicsBody: SCNPhysicsBody? { get set }
```

## Discussion

The default value is `nil`, specifying that the node does not participate in the physics simulation at all. If you provide a physics body, SceneKit updates the node’s position and orientation each time it processes a step of its physics simulation. For more information on SceneKit’s physics system, see SCNPhysicsWorld.

## See Also

### Adding Physics to a Node

var physicsField: SCNPhysicsField?

The physics field associated with the node.

