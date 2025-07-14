

- AppKit
- NSTreeNode
-  descendant(at:) 

Instance Method

# descendant(at:)

Returns the receiver’s descendant at the specified index path.

macOS 10.5+

``` source
func descendant(at indexPath: IndexPath) -> NSTreeNode?
```

## Parameters 

`indexPath`  

An index path specifying a descendant of the receiver.

## Return Value

A tree node, or `nil` if the node does not exist.

## See Also

### Getting information about a node

var representedObject: Any?

The object the tree node represents.

var indexPath: IndexPath

The position of the receiver relative to its root parent.

var isLeaf: Bool

A Boolean that indicates whether the receiver is a leaf node.

var children: [NSTreeNode]?

An array containing receiver’s child nodes.

var mutableChildren: NSMutableArray

A mutable array that provides read-write access to the receiver’s child nodes.

var parent: NSTreeNode?

The receiver’s parent node.

