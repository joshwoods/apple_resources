

- AppKit
- NSTreeNode
-  mutableChildren 

Instance Property

# mutableChildren

A mutable array that provides read-write access to the receiver’s child nodes.

macOS 10.5+

``` source
var mutableChildren: NSMutableArray { get }
```

## Discussion

Nodes that are inserted into this array have their parent nodes set to the receiver. Nodes that are removed from this array automatically have their parent node set to `nil`. The array that is returned is observable using key-value observing.

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

func descendant(at: IndexPath) -> NSTreeNode?

Returns the receiver’s descendant at the specified index path.

var parent: NSTreeNode?

The receiver’s parent node.

