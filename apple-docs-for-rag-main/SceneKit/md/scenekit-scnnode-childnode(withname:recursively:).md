

- SceneKit
- SCNNode
-  childNode(withName:recursively:) 

Instance Method

# childNode(withName:recursively:)

Returns the first node in the node’s child node subtree with the specified name.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func childNode(
    withName name: String,
    recursively: Bool
) -> SCNNode?
```

## Parameters 

`name`  

The name of the node to search for.

`recursively`  

true to search the entire child node subtree, or false to search only the node’s immediate children.

## Discussion

If the `recursive` parameter is true, SceneKit uses a preorder traversal to search the child node subtree—that is, the block searches a node before it searches each of the node’s children, and it searches all children of a node before searching any of that node’s sibling nodes. Otherwise, SceneKit searches only those nodes in the node’s childNodes array.

## See Also

### Searching the Node Hierarchy

func childNodes(passingTest: (SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> [SCNNode]

Returns all nodes in the node’s child node subtree that satisfy the test applied by a block.

func enumerateChildNodes((SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified block for each of the node’s child and descendant nodes.

func enumerateHierarchy((SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified block for each of the node’s child and descendant nodes, as well as for the node itself.

