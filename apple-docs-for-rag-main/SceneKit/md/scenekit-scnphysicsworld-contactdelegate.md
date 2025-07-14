

- SceneKit
- SCNPhysicsWorld
-  contactDelegate 

Instance Property

# contactDelegate

A delegate that is called when two physics bodies come in contact with each other.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
weak var contactDelegate: (any SCNPhysicsContactDelegate)? { get set }
```

## Discussion

A contact is created when two physics bodies overlap and one of the physics bodies has a collisionBitMask property that overlaps with the other body’s categoryBitMask property.

## See Also

### Detecting Contacts Between Physics Bodies

func contactTestBetween(SCNPhysicsBody, SCNPhysicsBody, options: [SCNPhysicsWorld.TestOption : Any]?) -> [SCNPhysicsContact]

Checks for contacts between two physics bodies.

func contactTest(with: SCNPhysicsBody, options: [SCNPhysicsWorld.TestOption : Any]?) -> [SCNPhysicsContact]

Checks for contacts between one physics body and any other bodies in the physics world.

