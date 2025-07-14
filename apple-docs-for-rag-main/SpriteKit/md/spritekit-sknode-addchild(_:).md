

- SpriteKit
- SKNode
-  addChild(\_:) 

Instance Method

# addChild(\_:)

Adds a node to the end of the receiver’s list of child nodes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func addChild(_ node: SKNode)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func addChild(_ node: SKNode)
```

## Parameters 

`node`  

The node to add. The node must not already have a parent.

## Mentioned in 

Accessing and Modifying the Node Tree

## See Also

### Modifying the Node Tree

Accessing and Modifying the Node Tree

See the objects and functions you use to control the node tree’s composition.

func insertChild(SKNode, at: Int)

Inserts a node into a specific position in the receiver’s list of child nodes.

func isEqual(to: SKNode) -> Bool

Compares the parameter node to the receiving node.

func move(toParent: SKNode)

Moves the node to a new parent node in the scene.

func removeFromParent()

Removes the receiving node from its parent.

func removeAllChildren()

Removes all of the node’s children.

func removeChildren(in: [SKNode])

Removes a list of children from the receiving node.

func inParentHierarchy(SKNode) -> Bool

Returns a Boolean value that indicates whether the node is a descendant of the target node.

