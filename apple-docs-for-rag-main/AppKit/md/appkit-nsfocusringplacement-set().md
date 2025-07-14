

- AppKit
- NSFocusRingPlacement
-  set() 

Instance Method

# set()

Specifies how the system draws the focus ring.

macOS

``` source
func set()
```

## Discussion

Use NSFocusRingPlacement.above to draw the focus ring over an image, use NSFocusRingPlacement.below to draw the focus ring under text, and use NSFocusRingPlacement.only if you don’t have an image or text. For the NSFocusRingPlacement.only case, fills a shape to add the focus ring around the shape.

Note that the focus ring may actually be drawn outside the view but will be clipped to any clipping superview or the window content view.

## See Also

### Drawing Focus Rings

enum NSFocusRingPlacement

Constants that indicate how the system draws the focus ring.

enum NSFocusRingType

Constants that describe the style of the focus ring.

