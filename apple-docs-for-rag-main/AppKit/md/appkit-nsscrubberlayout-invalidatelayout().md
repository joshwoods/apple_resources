

- AppKit
- NSScrubberLayout
-  invalidateLayout() 

Instance Method

# invalidateLayout()

Signals that the layout has been invalidated, and that the scrubber control should perform a new layout pass.

macOS 10.12.2+

``` source
@MainActor
func invalidateLayout()
```

## See Also

### Configuring a scrubber layout

class var layoutAttributesClass: AnyClass

A property containing a class that describes layout attributes.

var scrubber: NSScrubber?

The scrubber control that this layout is assigned to.

var visibleRect: NSRect

The currently visible rectangle, in the coordinate space of the scrubber content.

