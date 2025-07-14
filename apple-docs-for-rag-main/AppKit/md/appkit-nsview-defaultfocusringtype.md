

- AppKit
- NSView
-  defaultFocusRingType 

Type Property

# defaultFocusRingType

Returns the default focus ring type.

macOS

``` source
@MainActor
class var defaultFocusRingType: NSFocusRingType { get }
```

## Return Value

The default type of focus ring for objects of the view’s class. Possible return values are listed in NSFocusRingType.

## Discussion

If the value in the focusRingType property is NSFocusRingType.default, the view can call this class method to find out what type of focus ring is the default. The view is free to ignore the default setting.

## See Also

### Drawing the Focus Ring

var focusRingType: NSFocusRingType

The type of focus ring drawn around the view.

var focusRingMaskBounds: NSRect

The focus ring mask bounds, specified in the view’s coordinate space.

func drawFocusRingMask()

Draws the focus ring mask for the view.

func noteFocusRingMaskChanged()

Invoked to notify the view that the focus ring mask requires updating.

func setKeyboardFocusRingNeedsDisplay(NSRect)

Invalidates the area around the focus ring.

