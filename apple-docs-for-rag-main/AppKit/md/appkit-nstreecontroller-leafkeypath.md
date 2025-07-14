

- AppKit
- NSTreeController
-  leafKeyPath 

Instance Property

# leafKeyPath

The key path used by the tree controller to determine if a node is a leaf key.

macOS

``` source
var leafKeyPath: String? { get set }
```

## Discussion

Specifying a key path for this property is optional. If the tree controller is able to determine that a node is a leaf node, it can disable inserting or adding children to those nodes.

## See Also

### Specifying model attributes

var childrenKeyPath: String?

The key path used to find the children in the tree controller’s objects.

func childrenKeyPath(for: NSTreeNode) -> String?

Returns the key path used to find the children in the specified tree node.

var countKeyPath: String?

The key path used to find the number of children for a node.

func countKeyPath(for: NSTreeNode) -> String?

Returns the key path that provides the number of children for a specified node.

func leafKeyPath(for: NSTreeNode) -> String?

Returns the key path that specifies whether the node is a leaf node.

