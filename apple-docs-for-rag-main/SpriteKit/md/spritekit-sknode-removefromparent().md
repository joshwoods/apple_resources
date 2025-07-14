

- SpriteKit
- SKNode
-  removeFromParent() 

Instance Method

# removeFromParent()

Removes the receiving node from its parent.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func removeFromParent()
```

**watchOS**

``` source
func removeFromParent()
```

## Mentioned in 

Accessing and Modifying the Node Tree

Maximizing Node Drawing Performance

## See Also

### Modifying the Node Tree

Accessing and Modifying the Node Tree

See the objects and functions you use to control the node tree’s composition.

func addChild(SKNode)

Adds a node to the end of the receiver’s list of child nodes.

func insertChild(SKNode, at: Int)

Inserts a node into a specific position in the receiver’s list of child nodes.

func isEqual(to: SKNode) -> Bool

Compares the parameter node to the receiving node.

func move(toParent: SKNode)

Moves the node to a new parent node in the scene.

func removeAllChildren()

Removes all of the node’s children.

func removeChildren(in: [SKNode])

Removes a list of children from the receiving node.

func inParentHierarchy(SKNode) -> Bool

Returns a Boolean value that indicates whether the node is a descendant of the target node.

