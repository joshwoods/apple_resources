

- AppKit
- NSScrubberLayout
-  layoutAttributesForItem(at:) 

Instance Method

# layoutAttributesForItem(at:)

The layout attributes for the item with the specified index.

macOS 10.12.2+

``` source
@MainActor
func layoutAttributesForItem(at index: Int) -> NSScrubberLayoutAttributes?
```

## Discussion

The base implementation returns `nil`.

## See Also

### Subclassing a scrubber layout

func prepare()

Gives you an opportunity to perform layout calculations when the scrubber’s layout is invalidated.

var scrubberContentSize: NSSize

The size required to contain all elements within the scrubber.

func layoutAttributesForItems(in: NSRect) -> Set&lt;NSScrubberLayoutAttributes>

The set of layout attributes for all items within the provided rectangle.

var shouldInvalidateLayoutForSelectionChange: Bool

Determines whether the scrubber should refresh its layout when the selection changes.

var shouldInvalidateLayoutForHighlightChange: Bool

Determines whether the scrubber should refresh its layout when an item is highlighted.

func shouldInvalidateLayoutForChange(fromVisibleRect: NSRect, toVisibleRect: NSRect) -> Bool

Determines whether the scrubber should refresh its layout in response to a change of its visible region.

var automaticallyMirrorsInRightToLeftLayout: Bool

Determines whether the scrubber mirrors its layout for right-to-left layouts.

