

- SpriteKit
- SKNode
-  name 

Instance Property

# name

The node’s assignable name.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var name: String? { get set }
```

**watchOS**

``` source
var name: String? { get set }
```

## Mentioned in 

Searching the Node Tree

## Discussion

This property is used to identify a node in other parts of your game logic. For example, you might use this name as part of collision testing. You can also search for nodes in a tree by their name.

When choosing a name for a node, decide whether each node gets a unique name or whether some nodes will share a common name. If you give the node a unique name, you can find the node later by calling the childNode(withName:) method. If a name is shared by multiple nodes, the name usually means that these are all a similar object type in your game. In this case, you can iterate over those objects by calling the enumerateChildNodes(withName:using:) method.

## See Also

### Accessing Nodes by Name

Searching the Node Tree

Access nodes by name to avoid needing an instance variable.

func childNode(withName: String) -> SKNode?

Searches the children of the receiving node for a node with a specific name.

func enumerateChildNodes(withName: String, using: (SKNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Searches the children of the receiving node to perform processing for nodes that share a name.

subscript(String) -> [SKNode]

Returns an array of nodes that match the name parameter.

