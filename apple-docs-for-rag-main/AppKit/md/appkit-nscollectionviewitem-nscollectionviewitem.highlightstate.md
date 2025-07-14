

- AppKit
- NSCollectionViewItem
-  NSCollectionViewItem.HighlightState 

Enumeration

# NSCollectionViewItem.HighlightState

Constants indicating the type of highlight applied to an item.

macOS 10.11+

``` source
enum HighlightState
```

## Topics

### Constants

case none

No highlight state.

case forSelection

The selected highlight state. This type of highlight is applied when an item is selected. During interactive highlighting, this state is also applied to indicate that the item will become highlighted.

case forDeselection

The deselection highlight state. During interactive selection, this state is used to indicate that the item will become deselected when interactions end. After interactions end, the highlight state returns to NSCollectionViewItem.HighlightState.none.

case asDropTarget

The drop target highlight state. This type of highlight is applied when the item is the target of a drop operation on the collection view. After the drop operation completes, the highlight state returns to NSCollectionViewItem.HighlightState.none.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

