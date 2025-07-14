

- AppKit
-  NSScrubberLayout 

Class

# NSScrubberLayout

An abstract class that describes the layout of items within a scrubber control.

macOS 10.12.2+

``` source
@MainActor
class NSScrubberLayout
```

## Overview

To determine the layout of items in a scrubber, use one of the built-in subclasses (NSScrubberProportionalLayout or NSScrubberFlowLayout), or create a custom subclass to implement your own layout.

## Topics

### Creating a scrubber layout

init()

Initializes and returns a newly allocated scrubber layout object from code.

init(coder: NSCoder)

Initializes and returns a newly allocated scrubber layout object from a storyboard or nib file.

### Configuring a scrubber layout

class var layoutAttributesClass: AnyClass

A property containing a class that describes layout attributes.

var scrubber: NSScrubber?

The scrubber control that this layout is assigned to.

var visibleRect: NSRect

The currently visible rectangle, in the coordinate space of the scrubber content.

func invalidateLayout()

Signals that the layout has been invalidated, and that the scrubber control should perform a new layout pass.

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

var automaticallyMirrorsInRightToLeftLayout: Bool

Determines whether the scrubber mirrors its layout for right-to-left layouts.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSScrubberFlowLayout
- NSScrubberProportionalLayout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable

## See Also

### Scrubber layouts

class NSScrubberFlowLayout

A concrete layout object that arranges items end-to-end in a linear strip.

protocol NSScrubberFlowLayoutDelegate

A protocol that a scrubber delegate can adopt to provide the size of an item.

class NSScrubberProportionalLayout

A concrete layout object that sizes each item to some fraction of the scrubber’s visible size.

class NSScrubberLayoutAttributes

The layout of a scrubber item.

