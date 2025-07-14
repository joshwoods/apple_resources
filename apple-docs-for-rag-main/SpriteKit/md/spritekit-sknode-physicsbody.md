

- SpriteKit
- SKNode
-  physicsBody 

Instance Property

# physicsBody

The physics body associated with the node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var physicsBody: SKPhysicsBody? { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var physicsBody: SKPhysicsBody? { get set }
```

## Mentioned in 

Getting Started with Physics Bodies

Configuring a Physics Body

## Discussion

The default value is `nil`, which indicates that the node does not participate in the physics simulation at all. If a physics body is provided, when the scene’s physics are simulated, the physics body updates the node’s position and rotates the node.

## See Also

### Adding Physics Behaviors

Getting Started with Physics Bodies

Create and assign a physics body to enable physics.

