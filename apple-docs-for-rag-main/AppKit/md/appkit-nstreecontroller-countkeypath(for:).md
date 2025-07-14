

- AppKit
- NSTreeController
-  countKeyPath(for:) 

Instance Method

# countKeyPath(for:)

Returns the key path that provides the number of children for a specified node.

macOS 10.5+

``` source
func countKeyPath(for node: NSTreeNode) -> String?
```

## Parameters 

`node`  

A tree node in the tree controller’s content.

## Return Value

A string containing the key path in `node` that provides the number of children.

## See Also

### Specifying model attributes

var childrenKeyPath: String?

The key path used to find the children in the tree controller’s objects.

func childrenKeyPath(for: NSTreeNode) -> String?

Returns the key path used to find the children in the specified tree node.

var countKeyPath: String?

The key path used to find the number of children for a node.

var leafKeyPath: String?

The key path used by the tree controller to determine if a node is a leaf key.

func leafKeyPath(for: NSTreeNode) -> String?

Returns the key path that specifies whether the node is a leaf node.

