

- SpriteKit
- SKPhysicsBody
-  node 

Instance Property

# node

The node that this body is connected to.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
weak var node: SKNode? { get }
```

## Discussion

You associate the body with a node by assigning it to the physicsBody property of the SKNode object. If the body is not associated with a node, the value is `nil`.

