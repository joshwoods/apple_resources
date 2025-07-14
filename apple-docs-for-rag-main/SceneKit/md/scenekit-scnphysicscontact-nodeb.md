

- SceneKit
- SCNPhysicsContact
-  nodeB 

Instance Property

# nodeB

The node containing the second body in the contact.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var nodeB: SCNNode { get }
```

## Discussion

Use the node’s physicsBody property to examine physics characteristics of the node.

## See Also

### Inspecting the Contact Properties

var nodeA: SCNNode

The node containing the first body in the contact.

var contactPoint: SCNVector3

The contact point between the two physics bodies, in scene coordinates.

var contactNormal: SCNVector3

The normal vector at the contact point between the two physics bodies, in scene coordinates.

var collisionImpulse: CGFloat

The force over time of the collision, in newton-seconds.

var penetrationDistance: CGFloat

The distance of overlap, in units of scene coordinate space, between the two physics bodies.

