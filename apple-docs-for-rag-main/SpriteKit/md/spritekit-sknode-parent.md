

- SpriteKit
- SKNode
-  parent 

Instance Property

# parent

The node’s parent node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var parent: SKNode? { get }
```

**watchOS**

``` source
var parent: SKNode? { get }
```

## Mentioned in 

Accessing and Modifying the Node Tree

## Discussion

If the node is not in a node tree, the value is `nil`.

## See Also

### Accessing Related Nodes

About SpriteKit Coordinate Systems

Learn how a node conforms to its coordinate systems.

var scene: SKScene?

The scene node that contains this node.

var children: [SKNode]

The node’s children.

