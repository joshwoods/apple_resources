

- AppKit
- NSView
-  focusRingMaskBounds 

Instance Property

# focusRingMaskBounds

The focus ring mask bounds, specified in the view’s coordinate space.

macOS 10.7+

``` source
@MainActor
var focusRingMaskBounds: NSRect { get }
```

## Discussion

The rectangle in this property is specified relative to the view’s interior (bounds) coordinate space. The mask bounds allows the focus ring’s overall size and position to be determined before it is drawn. Override this property if your view requires the display of a focus ring. The default value of this property is NSZeroRect.

Note

The information provided by this property enables Accessibility to identify selected subelements for zoom tracking, so it is important that this method provide a reasonably tight bounding box and that the noteFocusRingMaskChanged() method is called as described.

## See Also

### Drawing the Focus Ring

var focusRingType: NSFocusRingType

The type of focus ring drawn around the view.

func drawFocusRingMask()

Draws the focus ring mask for the view.

func noteFocusRingMaskChanged()

Invoked to notify the view that the focus ring mask requires updating.

func setKeyboardFocusRingNeedsDisplay(NSRect)

Invalidates the area around the focus ring.

class var defaultFocusRingType: NSFocusRingType

Returns the default focus ring type.

