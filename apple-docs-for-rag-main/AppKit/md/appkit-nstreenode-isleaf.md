

- AppKit
- NSTreeNode
-  isLeaf 

Instance Property

# isLeaf

A Boolean that indicates whether the receiver is a leaf node.

macOS 10.5+

``` source
var isLeaf: Bool { get }
```

## Discussion

true if the receiver is a leaf node (has no child nodes), otherwise false.

## See Also

### Getting information about a node

var representedObject: Any?

The object the tree node represents.

var indexPath: IndexPath

The position of the receiver relative to its root parent.

var children: [NSTreeNode]?

An array containing receiver’s child nodes.

var mutableChildren: NSMutableArray

A mutable array that provides read-write access to the receiver’s child nodes.

func descendant(at: IndexPath) -> NSTreeNode?

Returns the receiver’s descendant at the specified index path.

var parent: NSTreeNode?

The receiver’s parent node.

