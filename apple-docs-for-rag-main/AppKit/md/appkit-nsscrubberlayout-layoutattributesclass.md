

- AppKit
- NSScrubberLayout
-  layoutAttributesClass 

Type Property

# layoutAttributesClass

A property containing a class that describes layout attributes.

macOS 10.12.2+

``` source
@MainActor
class var layoutAttributesClass: AnyClass { get }
```

## Return Value

The default return value is NSScrubberLayoutAttributes.

## Discussion

Create a custom subclass of NSScrubberLayout and override this method if you wish to use a custom layout attributes subclass.

## See Also

### Related Documentation

class NSScrubberLayoutAttributes

The layout of a scrubber item.

### Configuring a scrubber layout

var scrubber: NSScrubber?

The scrubber control that this layout is assigned to.

var visibleRect: NSRect

The currently visible rectangle, in the coordinate space of the scrubber content.

func invalidateLayout()

Signals that the layout has been invalidated, and that the scrubber control should perform a new layout pass.

