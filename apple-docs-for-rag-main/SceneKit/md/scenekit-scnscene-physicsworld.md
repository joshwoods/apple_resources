

- SceneKit
- SCNScene
-  physicsWorld 

Instance Property

# physicsWorld

The physics simulation associated with the scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var physicsWorld: SCNPhysicsWorld { get }
```

## Discussion

Every scene automatically creates a physics world object to simulate physics on nodes in the scene. You use this property to access the scene’s global physics properties, such as gravity, and to manage physics interactions between nodes. To make a node in the scene participate in the physics simulation, use either or both of its physicsBody and physicsField properties.

