

- SpriteKit
- SKNode
-  children 

Instance Property

# children

The node’s children.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var children: [SKNode] { get }
```

**watchOS**

``` source
var children: [SKNode] { get }
```

## Mentioned in 

Accessing and Modifying the Node Tree

Controlling User Interaction on Nodes

## Discussion

The objects in this array are all `SKNode` objects.

## See Also

### Accessing Related Nodes

About SpriteKit Coordinate Systems

Learn how a node conforms to its coordinate systems.

var scene: SKScene?

The scene node that contains this node.

var parent: SKNode?

The node’s parent node.

