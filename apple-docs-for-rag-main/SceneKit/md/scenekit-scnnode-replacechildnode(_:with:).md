

- SceneKit
- SCNNode
-  replaceChildNode(\_:with:) 

Instance Method

# replaceChildNode(\_:with:)

Removes a child from the node’s array of children and inserts another node in its place.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func replaceChildNode(
    _ oldChild: SCNNode,
    with newChild: SCNNode
)
```

## Parameters 

`oldChild`  

The existing child node to be replaced.

`newChild`  

The node with which to replace the child node.

Important

Raises an exception (invalidArgumentException) if `newChild` is `nil`.

## Discussion

If both the `oldChild` and `newChild` nodes are children of the node, calling this method swaps their positions in the array. Note that removing a node from the node hierarchy may result in it being deallocated.

Calling this method results in undefined behavior if the `oldChild` parameter doesn’t refer to a child of this node.

## See Also

### Managing the Node Hierarchy

var parent: SCNNode?

The node’s parent in the scene graph hierarchy.

var childNodes: [SCNNode]

An array of the node’s children in the scene graph hierarchy.

func addChildNode(SCNNode)

Adds a node to the node’s array of children.

func insertChildNode(SCNNode, at: Int)

Adds a node to the node’s array of children at a specified index.

func removeFromParentNode()

Removes the node from its parent’s array of child nodes.

