

- AppKit
- NSView
-  setKeyboardFocusRingNeedsDisplay(\_:) 

Instance Method

# setKeyboardFocusRingNeedsDisplay(\_:)

Invalidates the area around the focus ring.

macOS

``` source
@MainActor
func setKeyboardFocusRingNeedsDisplay(_ rect: NSRect)
```

## Parameters 

`rect`  

The rectangle of the control or cell defining the area around the focus ring. `rect` will be expanded to include the focus ring for invalidation.

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

class var defaultFocusRingType: NSFocusRingType

Returns the default focus ring type.

