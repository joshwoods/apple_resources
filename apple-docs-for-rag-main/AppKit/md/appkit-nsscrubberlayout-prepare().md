

- AppKit
- NSScrubberLayout
-  prepare() 

Instance Method

# prepare()

Gives you an opportunity to perform layout calculations when the scrubber’s layout is invalidated.

macOS 10.12.2+

``` source
@MainActor
func prepare()
```

## Discussion

Use this method in subclasses to perform layout calculations and caching in advance of rendering the scrubber.

The system calls this method when the scrubber’s layout is invalidated.

The base implementation of this method does nothing.

## See Also

### Subclassing a scrubber layout

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

func shouldInvalidateLayoutForChange(fromVisibleRect: NSRect, toVisibleRect: NSRect) -> Bool

Determines whether the scrubber should refresh its layout in response to a change of its visible region.

var automaticallyMirrorsInRightToLeftLayout: Bool

Determines whether the scrubber mirrors its layout for right-to-left layouts.

