

- AppKit
- NSTreeController
-  childrenKeyPath(for:) 

Instance Method

# childrenKeyPath(for:)

Returns the key path used to find the children in the specified tree node.

macOS 10.5+

``` source
func childrenKeyPath(for node: NSTreeNode) -> String?
```

## Parameters 

`node`  

A tree node in the tree controller’s content.

## Return Value

A string containing the key path in `node` that provides the child nodes.

## See Also

### Specifying model attributes

var childrenKeyPath: String?

The key path used to find the children in the tree controller’s objects.

var countKeyPath: String?

The key path used to find the number of children for a node.

func countKeyPath(for: NSTreeNode) -> String?

Returns the key path that provides the number of children for a specified node.

var leafKeyPath: String?

The key path used by the tree controller to determine if a node is a leaf key.

func leafKeyPath(for: NSTreeNode) -> String?

Returns the key path that specifies whether the node is a leaf node.

