

- AppKit
- NSScreen
-  backingAlignedRect(\_:options:) 

Instance Method

# backingAlignedRect(\_:options:)

Converts a rectangle in global screen coordinates to a pixel aligned rectangle.

macOS 10.7+

``` source
func backingAlignedRect(
    _ rect: NSRect,
    options: AlignmentOptions = []
) -> NSRect
```

## Parameters 

`rect`  

The input rectangle in global screen coordinates.

`options`  

Specifies the alignment options. See AlignmentOptions for possible values.

## Return Value

Returns a a pixel aligned rectangle on the target screen from the given input rectangle in global screen coordinates.

## Discussion

This method uses NSIntegralRectWithOptions(_:_:) to produce the pixel aligned rectangle.

## See Also

### Converting Between Screen and Backing Coordinates

var backingScaleFactor: CGFloat

The backing store pixel scale factor for the screen.

func convertRectFromBacking(NSRect) -> NSRect

Converts the rectangle from the device pixel aligned coordinates system of a screen.

func convertRectToBacking(NSRect) -> NSRect

Converts the rectangle to the device pixel aligned coordinates system of a screen.

