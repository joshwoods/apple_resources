

- AppKit
- NSTreeNode
-  children 

Instance Property

# children

An array containing receiver’s child nodes.

macOS 10.5+

``` source
var children: [NSTreeNode]? { get }
```

## See Also

### Getting information about a node

var representedObject: Any?

The object the tree node represents.

var indexPath: IndexPath

The position of the receiver relative to its root parent.

var isLeaf: Bool

A Boolean that indicates whether the receiver is a leaf node.

var mutableChildren: NSMutableArray

A mutable array that provides read-write access to the receiver’s child nodes.

func descendant(at: IndexPath) -> NSTreeNode?

Returns the receiver’s descendant at the specified index path.

var parent: NSTreeNode?

The receiver’s parent node.

