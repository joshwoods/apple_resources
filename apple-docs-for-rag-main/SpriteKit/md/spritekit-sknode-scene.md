

- SpriteKit
- SKNode
-  scene 

Instance Property

# scene

The scene node that contains this node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var scene: SKScene? { get }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var scene: SKScene? { get }
```

## Mentioned in 

Accessing and Modifying the Node Tree

## Discussion

If the node is not embedded in a scene, the value is `nil`.

## See Also

### Accessing Related Nodes

About SpriteKit Coordinate Systems

Learn how a node conforms to its coordinate systems.

var parent: SKNode?

The node’s parent node.

var children: [SKNode]

The node’s children.

