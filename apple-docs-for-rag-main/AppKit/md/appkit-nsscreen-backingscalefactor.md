

- AppKit
- NSScreen
-  backingScaleFactor 

Instance Property

# backingScaleFactor

The backing store pixel scale factor for the screen.

macOS 10.7+

``` source
var backingScaleFactor: CGFloat { get }
```

## Discussion

This is the scale factor representing the number of backing store pixels corresponding to each linear unit in screen space on this screen.

This method is provided for rare cases when the explicit scale factor is needed. As often as possible, you should use the NSView class’s convert backing methods.

## See Also

### Converting Between Screen and Backing Coordinates

func backingAlignedRect(NSRect, options: AlignmentOptions) -> NSRect

Converts a rectangle in global screen coordinates to a pixel aligned rectangle.

func convertRectFromBacking(NSRect) -> NSRect

Converts the rectangle from the device pixel aligned coordinates system of a screen.

func convertRectToBacking(NSRect) -> NSRect

Converts the rectangle to the device pixel aligned coordinates system of a screen.

