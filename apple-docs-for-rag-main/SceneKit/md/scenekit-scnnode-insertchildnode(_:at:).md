

- SceneKit
- SCNNode
-  insertChildNode(\_:at:) 

Instance Method

# insertChildNode(\_:at:)

Adds a node to the node’s array of children at a specified index.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func insertChildNode(
    _ child: SCNNode,
    at index: Int
)
```

## Parameters 

`child`  

The node to be inserted.

Important

Raises an exception (invalidArgumentException) if `child` is `nil`.

`index`  

The position at which to insert the new child node.

Important

Raises an exception (rangeException) if `index` is greater than the number of elements in the node’s childNodes array.

## See Also

### Managing the Node Hierarchy

var parent: SCNNode?

The node’s parent in the scene graph hierarchy.

var childNodes: [SCNNode]

An array of the node’s children in the scene graph hierarchy.

func addChildNode(SCNNode)

Adds a node to the node’s array of children.

func removeFromParentNode()

Removes the node from its parent’s array of child nodes.

func replaceChildNode(SCNNode, with: SCNNode)

Removes a child from the node’s array of children and inserts another node in its place.

