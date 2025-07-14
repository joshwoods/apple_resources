

- AppKit
- NSTreeController
-  selectionIndexPaths 

Instance Property

# selectionIndexPaths

An array containing the index paths of the currently selected objects.

macOS

``` source
var selectionIndexPaths: [IndexPath] { get }
```

## Discussion

This property contains an array containing NSIndexPath objects for each of the selected objects in the tree controller’s content. This property is observable using key-value observing.

## See Also

### Getting the current selection

func setSelectionIndexPath(IndexPath?) -> Bool

Sets the tree controller’s current selection.

var selectionIndexPath: IndexPath?

The index path of the first selected object.

func setSelectionIndexPaths([IndexPath]) -> Bool

Sets the tree controller’s current selection to the specified index paths.

var selectedObjects: [Any]

An array containing the currently selected objects in the tree controller’s content.

var selectedNodes: [NSTreeNode]

An array containing the tree controller’s selected tree nodes.

