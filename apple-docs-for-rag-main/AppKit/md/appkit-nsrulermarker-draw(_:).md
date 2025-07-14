

- AppKit
- NSRulerMarker
-  draw(\_:) 

Instance Method

# draw(\_:)

Draws the receiver’s image that appears in the supplied rectangle.

macOS

``` source
func draw(_ rect: NSRect)
```

## Parameters 

`rect`  

The rectangle to be drawn, in the ruler view’s coordinate system.

## See Also

### Related Documentation

var imageRectInRuler: NSRect

The rectangle occupied by the receiver’s image.

### Drawing and event handling

var isDragging: Bool

A Boolean that indicates whether the receiver is being dragged.

func trackMouse(with: NSEvent, adding: Bool) -> Bool

Handles user manipulation of the receiver in its ruler view.

