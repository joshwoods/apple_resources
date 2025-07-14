

- SceneKit
- SCNNode
-  enumerateChildNodes(\_:) 

Instance Method

# enumerateChildNodes(\_:)

Executes the specified block for each of the node’s child and descendant nodes.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func enumerateChildNodes(_ block: (SCNNode, UnsafeMutablePointer) -> Void)
```

## Parameters 

`block`  

The block to apply to the node’s child and descendant nodes.

- The block takes two parameters:

- child  
  The child node currently being evaluated.

stop  
A reference to a Boolean value. Set `*stop` to true in the block to abort further processing of the child node subtree.

## Discussion

SceneKit uses a recursive preorder traversal to process the child node subtree—that is, the block runs for a node before it runs for each of the node’s children, and it processes all children of a node before processing any of that node’s sibling nodes.

## See Also

### Searching the Node Hierarchy

func childNodes(passingTest: (SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> [SCNNode]

Returns all nodes in the node’s child node subtree that satisfy the test applied by a block.

func childNode(withName: String, recursively: Bool) -> SCNNode?

Returns the first node in the node’s child node subtree with the specified name.

func enumerateHierarchy((SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified block for each of the node’s child and descendant nodes, as well as for the node itself.

