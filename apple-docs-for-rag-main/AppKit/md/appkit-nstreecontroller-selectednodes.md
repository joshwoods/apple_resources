

- AppKit
- NSTreeController
-  selectedNodes 

Instance Property

# selectedNodes

An array containing the tree controller’s selected tree nodes.

macOS 10.5+

``` source
var selectedNodes: [NSTreeNode] { get }
```

## See Also

### Getting the current selection

func setSelectionIndexPath(IndexPath?) -> Bool

Sets the tree controller’s current selection.

var selectionIndexPath: IndexPath?

The index path of the first selected object.

func setSelectionIndexPaths([IndexPath]) -> Bool

Sets the tree controller’s current selection to the specified index paths.

var selectionIndexPaths: [IndexPath]

An array containing the index paths of the currently selected objects.

var selectedObjects: [Any]

An array containing the currently selected objects in the tree controller’s content.

