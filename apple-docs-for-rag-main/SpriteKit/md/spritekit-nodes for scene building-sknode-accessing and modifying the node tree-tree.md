

- SpriteKit
- Nodes for Scene Building
- SKNode
-  Accessing and Modifying the Node Tree 

Article

# Accessing and Modifying the Node Tree

See the objects and functions you use to control the node tree’s composition.

## Overview

You create the node tree by creating parent-child relationships between nodes. Each node maintains an ordered list of children, referenced by reading the node’s `children` property. The order of the children in the tree affects many aspects of scene processing, including hit testing and rendering, so it’s important to organize the node tree appropriately.

| Method | Description |
|----|----|
| addChild(_:) | Adds a node to the end of the receiver’s list of child nodes. |
| insertChild(_:at:) | Inserts a child into a specific position in the receiver’s list of child nodes. |
| removeFromParent() | Removes the receiving node from its parent. |

When you need to directly traverse the node tree, you use the properties in the following table to uncover the tree’s structure.

| Property | Description |
|----|----|
| children | The array of SKNode objects that are the receiving node’s children. |
| parent | If the node is a child of another node, this property holds the parent. Otherwise, it holds `nil`. |
| scene | If the node is included anywhere in a scene, this property returns the scene node that is the root of the tree. Otherwise it holds `nil`. |

## See Also

### Modifying the Node Tree

func addChild(SKNode)

Adds a node to the end of the receiver’s list of child nodes.

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

