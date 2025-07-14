

- AppKit
- NSScrubberLayout
-  shouldInvalidateLayoutForChange(fromVisibleRect:toVisibleRect:) 

Instance Method

# shouldInvalidateLayoutForChange(fromVisibleRect:toVisibleRect:)

Determines whether the scrubber should refresh its layout in response to a change of its visible region.

macOS 10.12.2+

``` source
@MainActor
func shouldInvalidateLayoutForChange(
    fromVisibleRect: NSRect,
    toVisibleRect: NSRect
) -> Bool
```

## Discussion

If true, the scrubber invalidates its layout in response to a change of the visible region, in response to a user scroll action, or to the scrubber being resized. Subclasses that rely on the size or origin of the visible region should return true.

The base implementation of this method returns false.

## See Also

### Subclassing a scrubber layout

func prepare()

Gives you an opportunity to perform layout calculations when the scrubber’s layout is invalidated.

var scrubberContentSize: NSSize

The size required to contain all elements within the scrubber.

func layoutAttributesForItem(at: Int) -> NSScrubberLayoutAttributes?

The layout attributes for the item with the specified index.

func layoutAttributesForItems(in: NSRect) -> Set&lt;NSScrubberLayoutAttributes>

The set of layout attributes for all items within the provided rectangle.

var shouldInvalidateLayoutForSelectionChange: Bool

Determines whether the scrubber should refresh its layout when the selection changes.

var shouldInvalidateLayoutForHighlightChange: Bool

Determines whether the scrubber should refresh its layout when an item is highlighted.

var automaticallyMirrorsInRightToLeftLayout: Bool

Determines whether the scrubber mirrors its layout for right-to-left layouts.

