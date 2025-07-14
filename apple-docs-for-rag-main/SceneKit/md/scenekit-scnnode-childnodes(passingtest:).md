

- SceneKit
- SCNNode
-  childNodes(passingTest:) 

Instance Method

# childNodes(passingTest:)

Returns all nodes in the node’s child node subtree that satisfy the test applied by a block.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func childNodes(passingTest predicate: (SCNNode, UnsafeMutablePointer) -> Bool) -> [SCNNode]
```

## Parameters 

`predicate`  

The block to apply to the node’s child and descendant nodes.

- The block takes two parameters:

- child  
  The child node currently being searched.

stop  
A reference to a Boolean value. Set `*stop` to true in the block to abort further processing of the child node subtree.

- The block returns a Boolean value indicating whether to include the `child` node in the search results array.

## Return Value

An array containing nodes that passed the test.

## Discussion

Use this method to search for nodes using a test you specify. For example, you can search for empty nodes using a block that returns YES for nodes whose light, camera, and geometry properties are all `nil`.

SceneKit uses a recursive preorder traversal to search the child node subtree—that is, the block searches a node before it searches each of the node’s children, and it searches all children of a node before searching any of that node’s sibling nodes.

## See Also

### Searching the Node Hierarchy

func childNode(withName: String, recursively: Bool) -> SCNNode?

Returns the first node in the node’s child node subtree with the specified name.

func enumerateChildNodes((SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified block for each of the node’s child and descendant nodes.

func enumerateHierarchy((SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified block for each of the node’s child and descendant nodes, as well as for the node itself.

