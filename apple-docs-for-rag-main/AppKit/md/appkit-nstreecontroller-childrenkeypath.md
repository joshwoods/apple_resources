

- AppKit
- NSTreeController
-  childrenKeyPath 

Instance Property

# childrenKeyPath

The key path used to find the children in the tree controller’s objects.

macOS

``` source
var childrenKeyPath: String? { get set }
```

## Discussion

The default value of this property is `nil`.

## See Also

### Specifying model attributes

func childrenKeyPath(for: NSTreeNode) -> String?

Returns the key path used to find the children in the specified tree node.

var countKeyPath: String?

The key path used to find the number of children for a node.

func countKeyPath(for: NSTreeNode) -> String?

Returns the key path that provides the number of children for a specified node.

var leafKeyPath: String?

The key path used by the tree controller to determine if a node is a leaf key.

func leafKeyPath(for: NSTreeNode) -> String?

Returns the key path that specifies whether the node is a leaf node.

