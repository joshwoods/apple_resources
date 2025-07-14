

- AppKit
- NSScrubberLayout
-  visibleRect 

Instance Property

# visibleRect

The currently visible rectangle, in the coordinate space of the scrubber content.

macOS 10.12.2+

``` source
@MainActor
var visibleRect: NSRect { get }
```

## Discussion

The value of this property is NSZeroRect if the layout is not currently assigned to a scrubber control.

## See Also

### Configuring a scrubber layout

class var layoutAttributesClass: AnyClass

A property containing a class that describes layout attributes.

var scrubber: NSScrubber?

The scrubber control that this layout is assigned to.

func invalidateLayout()

Signals that the layout has been invalidated, and that the scrubber control should perform a new layout pass.

