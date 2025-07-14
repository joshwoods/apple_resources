

- SceneKit
- SCNNode
-  physicsField 

Instance Property

# physicsField

The physics field associated with the node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var physicsField: SCNPhysicsField? { get set }
```

## Discussion

Physics fields apply forces to other physics bodies in a specified area around their node. For example, a SCNPhysicsDragField field slows all physics bodies that pass through its area. For a full list of field types and their effects, see SCNPhysicsField.

A node can contain both a physics body that defines collision behavior and a physics field that defines forces in its area. For example, two nodes containing physics bodies and radial gravity fields will be attracted to one another, but will bounce off each other when they collide.

## See Also

### Adding Physics to a Node

var physicsBody: SCNPhysicsBody?

The physics body associated with the node.

