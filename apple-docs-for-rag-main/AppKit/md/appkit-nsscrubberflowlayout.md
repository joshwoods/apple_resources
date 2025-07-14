

- AppKit
-  NSScrubberFlowLayout 

Class

# NSScrubberFlowLayout

A concrete layout object that arranges items end-to-end in a linear strip.

macOS 10.12.2+

``` source
@MainActor
class NSScrubberFlowLayout
```

## Overview

To set the size of items on a per-item basis, ensure that your scrubber delegate conforms to the NSScrubberFlowLayoutDelegate protocol, and provides an implementation of the scrubber(_:layout:sizeForItemAt:) method.

## Topics

### Configuring the layout

var itemSpacing: CGFloat

The horizontal spacing between items, specified in points.

var itemSize: NSSize

The frame size for each item in the scrubber.

### Invalidating the layout

func invalidateLayoutForItems(at: IndexSet)

Informs the scrubber that it should perform a new layout pass for the items at the specified indexes.

## Relationships

### Inherits From

- NSScrubberLayout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol

## See Also

### Scrubber layouts

protocol NSScrubberFlowLayoutDelegate

A protocol that a scrubber delegate can adopt to provide the size of an item.

class NSScrubberProportionalLayout

A concrete layout object that sizes each item to some fraction of the scrubber’s visible size.

class NSScrubberLayoutAttributes

The layout of a scrubber item.

class NSScrubberLayout

An abstract class that describes the layout of items within a scrubber control.

