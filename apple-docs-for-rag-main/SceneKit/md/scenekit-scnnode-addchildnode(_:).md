

- SceneKit
- SCNNode
-  addChildNode(\_:) 

Instance Method

# addChildNode(\_:)

Adds a node to the node’s array of children.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func addChildNode(_ child: SCNNode)
```

## Parameters 

`child`  

The node to be added.

## Discussion

Calling this method appends the node to the end of the childNodes array.

## See Also

### Managing the Node Hierarchy

var parent: SCNNode?

The node’s parent in the scene graph hierarchy.

var childNodes: [SCNNode]

An array of the node’s children in the scene graph hierarchy.

func insertChildNode(SCNNode, at: Int)

Adds a node to the node’s array of children at a specified index.

func removeFromParentNode()

Removes the node from its parent’s array of child nodes.

func replaceChildNode(SCNNode, with: SCNNode)

Removes a child from the node’s array of children and inserts another node in its place.

