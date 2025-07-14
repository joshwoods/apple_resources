

- AppKit
- NSScreen
-  convertRectToBacking(\_:) 

Instance Method

# convertRectToBacking(\_:)

Converts the rectangle to the device pixel aligned coordinates system of a screen.

macOS 10.7+

``` source
func convertRectToBacking(_ rect: NSRect) -> NSRect
```

## Parameters 

`rect`  

The rectangle.

## Return Value

The rectangle converted to the device pixel aligned coordinates system of the screen.

## See Also

### Converting Between Screen and Backing Coordinates

func backingAlignedRect(NSRect, options: AlignmentOptions) -> NSRect

Converts a rectangle in global screen coordinates to a pixel aligned rectangle.

var backingScaleFactor: CGFloat

The backing store pixel scale factor for the screen.

func convertRectFromBacking(NSRect) -> NSRect

Converts the rectangle from the device pixel aligned coordinates system of a screen.

