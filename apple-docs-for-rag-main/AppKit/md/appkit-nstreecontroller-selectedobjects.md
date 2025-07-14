

- AppKit
- NSTreeController
-  selectedObjects 

Instance Property

# selectedObjects

An array containing the currently selected objects in the tree controller’s content.

macOS

``` source
var selectedObjects: [Any] { get }
```

## Discussion

This property is observable using key-value observing.

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

var selectedNodes: [NSTreeNode]

An array containing the tree controller’s selected tree nodes.

