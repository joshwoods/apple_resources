

- SpriteKit
-  SKPhysicsContactDelegate 

Protocol

# SKPhysicsContactDelegate

Methods your app can implement to respond when physics bodies come into contact.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol SKPhysicsContactDelegate : NSObjectProtocol
```

## Mentioned in 

Responding to Frame-Cycle Events

Getting Started with Physics

## Overview

An object that implements the SKPhysicsContactDelegate protocol can respond when two physics bodies with overlapping contactTestBitMask values are in contact with each other in a physics world. To receive contact messages, you set the contactDelegate property of a SKPhysicsWorld object. The delegate is called when a contact starts or ends.

Important

The physics contact delegate methods are called during the physics simulation step. During that time, the physics world can’t be modified and the behavior of any changes to the physics bodies in the simulation is undefined. If you need to make such changes, set a flag inside didBegin(_:) or didEnd(_:) and make changes in response to that flag in the update(_:for:) method in a SKSceneDelegate.

You can use the contact delegate to play a sound or execute game logic, such as increasing a player’s score, when a contact event occurs. The following code shows how to display a shockwave effect when two nodes with the name `ball` come into contact. The code only creates the effect when the collision impulse is above a specified threshold:

Listing 1. Creating a shockwave effect when objects come into contact

```
let shockWaveAction: SKAction = {
    let growAndFadeAction = SKAction.group([SKAction.scale(to: 50, duration: 0.5),
                                            SKAction.fadeOut(withDuration: 0.5)])

    let sequence = SKAction.sequence([growAndFadeAction,
                                      SKAction.removeFromParent()])

    return sequence
}()

func didBegin(_ contact: SKPhysicsContact) {
    if contact.collisionImpulse > 5 &&
        contact.bodyA.node?.name == "ball" &&
        contact.bodyB.node?.name == "ball" {

        let shockwave = SKShapeNode(circleOfRadius: 1)

        shockwave.position = contact.contactPoint
        scene.addChild(shockwave)

        shockwave.run(shockWaveAction)
    }
}
```

## Topics

### Responding to Contact Events

func didBegin(SKPhysicsContact)

Called when two bodies first contact each other.

func didEnd(SKPhysicsContact)

Called when the contact ends between two physics bodies.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Physics Simulation

Getting Started with Physics

Simulate gravity, acceleration, collision detection, or joints.

class SKPhysicsWorld

The driver of the physics engine in a scene; it exposes the ability for you to configure and query the physics system.

class SKPhysicsBody

An object that adds physics simulation to a node.

class SKPhysicsContact

A description of the contact between two physics bodies.

class SKFieldNode

A node that applies physics effects to nearby nodes.

