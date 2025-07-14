

- AppKit
- NSTreeController
-  setSelectionIndexPaths(\_:) 

Instance Method

# setSelectionIndexPaths(\_:)

Sets the tree controller’s current selection to the specified index paths.

macOS

``` source
func setSelectionIndexPaths(_ indexPaths: [IndexPath]) -> Bool
```

## Parameters 

`indexPaths`  

An array of NSIndexPath objects specifying the selected objects.

## Return Value

Return true if the selection has changed, otherwise false.

## Discussion

Attempting to change the selection may cause a `commitEditing` message which fails, thus denying the selection change.

## See Also

### Getting the current selection

func setSelectionIndexPath(IndexPath?) -> Bool

Sets the tree controller’s current selection.

var selectionIndexPath: IndexPath?

The index path of the first selected object.

var selectionIndexPaths: [IndexPath]

An array containing the index paths of the currently selected objects.

var selectedObjects: [Any]

An array containing the currently selected objects in the tree controller’s content.

var selectedNodes: [NSTreeNode]

An array containing the tree controller’s selected tree nodes.

