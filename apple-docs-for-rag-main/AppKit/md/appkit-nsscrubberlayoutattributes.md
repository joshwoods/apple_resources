

- AppKit
-  NSScrubberLayoutAttributes 

Class

# NSScrubberLayoutAttributes

The layout of a scrubber item.

macOS 10.12.2+

``` source
class NSScrubberLayoutAttributes
```

## Overview

A layout attributes object is the model for the layout of a single item in a scrubber control.

If you require model attributes in addition to those provided by this class, create a subclass and add appropriate attributes. Subclasses must implement isEqual(_:), hash and the NSCopying protocol.

## Topics

### Creating layout attributes

convenience init(forItemAt: Int)

Creates a new layout attributes object for the specified scrubber item index.

### Controlling the layout

var alpha: CGFloat

The item’s alpha value.

var frame: NSRect

The frame of the scrubber item.

var itemIndex: Int

The index of the scrubber item that is represented by the item’s layout attributes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Scrubber layouts

class NSScrubberFlowLayout

A concrete layout object that arranges items end-to-end in a linear strip.

protocol NSScrubberFlowLayoutDelegate

A protocol that a scrubber delegate can adopt to provide the size of an item.

class NSScrubberProportionalLayout

A concrete layout object that sizes each item to some fraction of the scrubber’s visible size.

class NSScrubberLayout

An abstract class that describes the layout of items within a scrubber control.

