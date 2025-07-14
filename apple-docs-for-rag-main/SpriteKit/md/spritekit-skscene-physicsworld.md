

- SpriteKit
- SKScene
-  physicsWorld 

Instance Property

# physicsWorld

The physics simulation associated with the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var physicsWorld: SKPhysicsWorld { get }
```

**watchOS**

``` source
var physicsWorld: SKPhysicsWorld { get }
```

## Discussion

Every scene automatically creates a physics world object to simulate physics on nodes in the scene. You use this property to access the scene’s global physics properties, such as gravity. To add physics to a particular node, see physicsBody.

