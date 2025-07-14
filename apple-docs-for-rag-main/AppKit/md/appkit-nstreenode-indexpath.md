

- AppKit
- NSTreeNode
-  indexPath 

Instance Property

# indexPath

The position of the receiver relative to its root parent.

macOS 10.5+

``` source
var indexPath: IndexPath { get }
```

## See Also

### Getting information about a node

var representedObject: Any?

The object the tree node represents.

var isLeaf: Bool

A Boolean that indicates whether the receiver is a leaf node.

var children: [NSTreeNode]?

An array containing receiver’s child nodes.

var mutableChildren: NSMutableArray

A mutable array that provides read-write access to the receiver’s child nodes.

func descendant(at: IndexPath) -> NSTreeNode?

Returns the receiver’s descendant at the specified index path.

var parent: NSTreeNode?

The receiver’s parent node.

