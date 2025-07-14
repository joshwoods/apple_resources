

- AppKit
- NSCollectionViewItem
- NSCollectionViewItem.HighlightState
-  NSCollectionViewItem.HighlightState.forDeselection 

Case

# NSCollectionViewItem.HighlightState.forDeselection

The deselection highlight state. During interactive selection, this state is used to indicate that the item will become deselected when interactions end. After interactions end, the highlight state returns to NSCollectionViewItem.HighlightState.none.

macOS 10.11+

``` source
case forDeselection
```

## See Also

### Constants

case none

No highlight state.

case forSelection

The selected highlight state. This type of highlight is applied when an item is selected. During interactive highlighting, this state is also applied to indicate that the item will become highlighted.

case asDropTarget

The drop target highlight state. This type of highlight is applied when the item is the target of a drop operation on the collection view. After the drop operation completes, the highlight state returns to NSCollectionViewItem.HighlightState.none.

