

- AppKit
- NSTreeController
-  setSelectionIndexPath(\_:) 

Instance Method

# setSelectionIndexPath(\_:)

Sets the tree controller’s current selection.

macOS

``` source
func setSelectionIndexPath(_ indexPath: IndexPath?) -> Bool
```

## Parameters 

`indexPath`  

The proposed new selection.

## Return Value

Return true if the selection has changed, otherwise false.

## Discussion

Attempting to change the selection may cause a `commitEditing` message which fails, thus denying the selection change.

## See Also

### Getting the current selection

var selectionIndexPath: IndexPath?

The index path of the first selected object.

func setSelectionIndexPaths([IndexPath]) -> Bool

Sets the tree controller’s current selection to the specified index paths.

var selectionIndexPaths: [IndexPath]

An array containing the index paths of the currently selected objects.

var selectedObjects: [Any]

An array containing the currently selected objects in the tree controller’s content.

var selectedNodes: [NSTreeNode]

An array containing the tree controller’s selected tree nodes.

