

- AppKit
- NSCollectionViewItem
-  isSelected 

Instance Property

# isSelected

A Boolean indicating whether the item is currently selected.

macOS 10.5+

``` source
@MainActor
var isSelected: Bool { get set }
```

## Discussion

The value of this property is true when the item is selected or false when it is not.

## See Also

### Managing the Selection and Highlight States

var highlightState: NSCollectionViewItem.HighlightState

The highlight state currently applied to the item.

