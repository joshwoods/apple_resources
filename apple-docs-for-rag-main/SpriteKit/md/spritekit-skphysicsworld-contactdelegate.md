

- SpriteKit
- SKPhysicsWorld
-  contactDelegate 

Instance Property

# contactDelegate

A delegate that is called when two physics bodies come in contact with each other.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
unowned(unsafe) var contactDelegate: (any SKPhysicsContactDelegate)? { get set }
```

## Discussion

A contact is created when two physics bodies overlap and one of the physics bodies has a contactTestBitMask property that overlaps with the other body’s categoryBitMask property. By default, a physics body’s contactTestBitMask is set to all bits cleared.

