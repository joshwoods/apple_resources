

- AppKit
- NSTreeNode
-  representedObject 

Instance Property

# representedObject

The object the tree node represents.

macOS 10.5+

``` source
var representedObject: Any? { get }
```

## See Also

### Getting information about a node

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

var parent: NSTreeNode?

The receiver’s parent node.

