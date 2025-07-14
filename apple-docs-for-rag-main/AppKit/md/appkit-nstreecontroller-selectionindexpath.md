

- AppKit
- NSTreeController
-  selectionIndexPath 

Instance Property

# selectionIndexPath

The index path of the first selected object.

macOS

``` source
var selectionIndexPath: IndexPath? { get }
```

## Discussion

The value of this property is `nil` if there is no selection. This property is observable using key-value observing.

## See Also

### Getting the current selection

func setSelectionIndexPath(IndexPath?) -> Bool

Sets the tree controller’s current selection.

func setSelectionIndexPaths([IndexPath]) -> Bool

Sets the tree controller’s current selection to the specified index paths.

var selectionIndexPaths: [IndexPath]

An array containing the index paths of the currently selected objects.

var selectedObjects: [Any]

An array containing the currently selected objects in the tree controller’s content.

var selectedNodes: [NSTreeNode]

An array containing the tree controller’s selected tree nodes.

