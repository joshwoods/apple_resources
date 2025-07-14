

- SceneKit
- SCNNode
-  parent 

Instance Property

# parent

The node’s parent in the scene graph hierarchy.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var parent: SCNNode? { get }
```

## Discussion

For a scene’s rootNode object, the value of this property is `nil`.

## See Also

### Managing the Node Hierarchy

var childNodes: [SCNNode]

An array of the node’s children in the scene graph hierarchy.

func addChildNode(SCNNode)

Adds a node to the node’s array of children.

func insertChildNode(SCNNode, at: Int)

Adds a node to the node’s array of children at a specified index.

func removeFromParentNode()

Removes the node from its parent’s array of child nodes.

func replaceChildNode(SCNNode, with: SCNNode)

Removes a child from the node’s array of children and inserts another node in its place.

