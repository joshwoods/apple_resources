

- SceneKit
- SCNNode
-  removeFromParentNode() 

Instance Method

# removeFromParentNode()

Removes the node from its parent’s array of child nodes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func removeFromParentNode()
```

## Discussion

Removing nodes from the node hierarchy serves two purposes. Nodes own their contents (child nodes or attached lights, geometries, and other objects), so deallocating unneeded nodes can reduce memory usage. Additionally, SceneKit does more work at rendering time with a large, complex node hierarchy, so removing nodes whose contents you don’t need to display can improve rendering performance.

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

func replaceChildNode(SCNNode, with: SCNNode)

Removes a child from the node’s array of children and inserts another node in its place.

