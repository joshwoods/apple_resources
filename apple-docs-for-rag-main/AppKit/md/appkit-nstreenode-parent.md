

- AppKit
- NSTreeNode
-  parent 

Instance Property

# parent

The receiver’s parent node.

macOS 10.5+

``` source
weak var parent: NSTreeNode? { get }
```

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

func descendant(at: IndexPath) -> NSTreeNode?

Returns the receiver’s descendant at the specified index path.

