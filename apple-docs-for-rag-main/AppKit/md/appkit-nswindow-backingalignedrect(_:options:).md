

- AppKit
- NSWindow
-  backingAlignedRect(\_:options:) 

Instance Method

# backingAlignedRect(\_:options:)

Returns a backing store pixel-aligned rectangle in window coordinates.

macOS 10.7+

``` source
@MainActor
func backingAlignedRect(
    _ rect: NSRect,
    options: AlignmentOptions = []
) -> NSRect
```

## Parameters 

`rect`  

The rectangle in view coordinates.

`options`  

The alignment options. AlignmentOptions specifies the possible values.

## Return Value

A rectangle, in window coordinates, aligned to the backing store pixels according to the specified options.

## Discussion

This method uses NSIntegralRectWithOptions(_:_:) to align the input rectangle, and produces a backing store pixel-aligned rectangle.

## See Also

### Converting Coordinates

var backingScaleFactor: CGFloat

The backing scale factor.

func convertFromBacking(NSRect) -> NSRect

Converts a rectangle from its pixel-aligned backing store coordinate system to the window’s coordinate system.

func convertFromScreen(NSRect) -> NSRect

Converts a rectangle from the screen coordinate system to the window’s coordinate system.

func convertPointFromBacking(NSPoint) -> NSPoint

Converts a point from its pixel-aligned backing store coordinate system to the window’s coordinate system.

func convertPoint(fromScreen: NSPoint) -> NSPoint

Converts a point from the screen coordinate system to the window’s coordinate system.

func convertToBacking(NSRect) -> NSRect

Converts a rectangle from the window’s coordinate system to its pixel-aligned backing store coordinate system.

func convertToScreen(NSRect) -> NSRect

Converts a rectangle to the screen coordinate system from the window’s coordinate system.

func convertPointToBacking(NSPoint) -> NSPoint

Converts a point from the window’s coordinate system to its pixel-aligned backing store coordinate system.

func convertPoint(toScreen: NSPoint) -> NSPoint

Converts a point to the screen coordinate system from the window’s coordinate system.

