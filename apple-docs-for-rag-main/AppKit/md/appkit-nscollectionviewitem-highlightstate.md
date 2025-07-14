

- AppKit
- NSCollectionViewItem
-  highlightState 

Instance Property

# highlightState

The highlight state currently applied to the item.

macOS 10.11+

``` source
@MainActor
var highlightState: NSCollectionViewItem.HighlightState { get set }
```

## Discussion

The highlight state provides a visual indication of operations happening to items in the collection view. The highlight state normally toggles between the NSCollectionViewItem.HighlightState.none and NSCollectionViewItem.HighlightState.forSelection states, but other states may be applied to indicate transient conditions. For example, the NSCollectionViewItem.HighlightState.forDeselection state is applied during interactive selections when a currently selected item is about to be deselected.

## See Also

### Managing the Selection and Highlight States

var isSelected: Bool

A Boolean indicating whether the item is currently selected.

