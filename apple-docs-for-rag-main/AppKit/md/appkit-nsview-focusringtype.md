

- AppKit
- NSView
-  focusRingType 

Instance Property

# focusRingType

The type of focus ring drawn around the view.

macOS

``` source
@MainActor
var focusRingType: NSFocusRingType { get set }
```

## Return Value

An `enum` constant identifying a type of focus ring. Possible values are listed in NSFocusRingType.

## Discussion

Use this property to specify the type of focus ring to draw. For a list of possible values, see NSFocusRingType.

To disable drawing of a view’s focus ring, set the value of this property to NSFocusRingType.none. You should only disable the default drawing of a view’s focus ring when you want the view to draw its own focus ring. For example, you might disable focus ring drawing when the view uses its background color to indicate focus or when the view does not have sufficient space to display a focus ring.

Changing the value in this property does not cause the view to draw the actual focus ring. You are responsible for drawing the focus ring in your view’s draw(_:) method whenever your view is made the first responder.

To ensure the correct redrawing of focus rings, note that AppKit may automatically draw parts of a window in addition to those that are marked as needing display. For example, AppKit may redraw parts of the first responder view in an app’s key window, if that view’s focusRingType property is set to a value other than NSFocusRingType.none. If your view can become first responder, but doesn’t draw a focus ring, set focusRingType to NSFocusRingType.none to prevent AppKit from unnecessarily redrawing the view’s focus ring.

## See Also

### Drawing the Focus Ring

var focusRingMaskBounds: NSRect

The focus ring mask bounds, specified in the view’s coordinate space.

func drawFocusRingMask()

Draws the focus ring mask for the view.

func noteFocusRingMaskChanged()

Invoked to notify the view that the focus ring mask requires updating.

func setKeyboardFocusRingNeedsDisplay(NSRect)

Invalidates the area around the focus ring.

class var defaultFocusRingType: NSFocusRingType

Returns the default focus ring type.

