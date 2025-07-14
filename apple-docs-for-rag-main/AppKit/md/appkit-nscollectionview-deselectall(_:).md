

- AppKit
- NSCollectionView
-  deselectAll(\_:) 

Instance Method

# deselectAll(\_:)

Deselects all items in the collection view.

macOS 10.5+

``` source
@IBAction @MainActor
func deselectAll(_ sender: Any?)
```

## Parameters 

`sender`  

The object that requested the action. You may specify `nil` for this property.

## Discussion

This method works only when the isSelectable and allowsEmptySelection properties are both true true. If either property is set to false, this method quietly does nothing and any connected menu item is disabled.

This method consults the delegate object regarding the selection. Specifically, it calls the delegate’s collectionView(_:shouldDeselectItemsAt:) method to see if the items should be selected. For any items that are selected, it calls the collectionView(_:didDeselectItemsAt:) method.

## See Also

### Managing the Selection

var isSelectable: Bool

A Boolean value that indicates whether the user may select items in the collection view.

var allowsMultipleSelection: Bool

A Boolean value that indicates whether the user may select more than one item in the collection view.

var allowsEmptySelection: Bool

A Boolean value indicating whether the collection view may have no selected items.

var selectionIndexPaths: Set&lt;IndexPath>

The set of index paths representing the currently selected items.

func selectAll(Any?)

Selects all items in the collection view, if doing so is possible.

func selectItems(at: Set&lt;IndexPath>, scrollPosition: NSCollectionView.ScrollPosition)

Adds the specified items to the current selection and optionally scrolls the items into position.

func deselectItems(at: Set&lt;IndexPath>)

Removes the specified items from the current selection.

