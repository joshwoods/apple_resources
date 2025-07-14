

- AppKit
- NSScrubberLayout
-  automaticallyMirrorsInRightToLeftLayout 

Instance Property

# automaticallyMirrorsInRightToLeftLayout

Determines whether the scrubber mirrors its layout for right-to-left layouts.

macOS 10.12.2+

``` source
@MainActor
var automaticallyMirrorsInRightToLeftLayout: Bool { get }
```

## Discussion

If true, the layout of a scrubber in a right-to-left interface is the mirror of the left-to-right version. If you wish to customize the behavior of the scrubber in right-to-left interfaces in a custom subclass, override this method to return false.

The base implementation of this method returns true.

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

func shouldInvalidateLayoutForChange(fromVisibleRect: NSRect, toVisibleRect: NSRect) -> Bool

Determines whether the scrubber should refresh its layout in response to a change of its visible region.

