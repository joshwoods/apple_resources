

- AppKit
-  NSScrubberProportionalLayout 

Class

# NSScrubberProportionalLayout

A concrete layout object that sizes each item to some fraction of the scrubber’s visible size.

macOS 10.12.2+

``` source
@MainActor
class NSScrubberProportionalLayout
```

## Topics

### Initializing a proprotional layout

init(numberOfVisibleItems: Int)

Initializes and returns a newly allocated proportional layout, configured to display the given number of items.

init(coder: NSCoder)

Initializes and returns a newly allocated proprotional layout object from a storyboard or nib file.

### Configuring the layout

var numberOfVisibleItems: Int

The number of items visible in the scrubber at once.

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
- Sendable

## See Also

### Scrubber layouts

class NSScrubberFlowLayout

A concrete layout object that arranges items end-to-end in a linear strip.

protocol NSScrubberFlowLayoutDelegate

A protocol that a scrubber delegate can adopt to provide the size of an item.

class NSScrubberLayoutAttributes

The layout of a scrubber item.

class NSScrubberLayout

An abstract class that describes the layout of items within a scrubber control.

