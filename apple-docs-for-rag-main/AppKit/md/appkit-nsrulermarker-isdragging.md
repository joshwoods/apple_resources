

- AppKit
- NSRulerMarker
-  isDragging 

Instance Property

# isDragging

A Boolean that indicates whether the receiver is being dragged.

macOS

``` source
var isDragging: Bool { get }
```

## Discussion

true if the receiver is being dragged, false otherwise.

## See Also

### Drawing and event handling

func draw(NSRect)

Draws the receiver’s image that appears in the supplied rectangle.

func trackMouse(with: NSEvent, adding: Bool) -> Bool

Handles user manipulation of the receiver in its ruler view.

