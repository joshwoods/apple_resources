

- AppKit
- NSScrubberLayout
-  scrubber 

Instance Property

# scrubber

The scrubber control that this layout is assigned to.

macOS 10.12.2+

``` source
@MainActor
weak var scrubber: NSScrubber? { get }
```

## Discussion

If this layout is not currently assigned to a scrubber control, the value of this property is `nil`.

## See Also

### Configuring a scrubber layout

class var layoutAttributesClass: AnyClass

A property containing a class that describes layout attributes.

var visibleRect: NSRect

The currently visible rectangle, in the coordinate space of the scrubber content.

func invalidateLayout()

Signals that the layout has been invalidated, and that the scrubber control should perform a new layout pass.

