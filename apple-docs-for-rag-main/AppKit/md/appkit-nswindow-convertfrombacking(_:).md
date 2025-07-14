

- AppKit
- NSWindow
-  convertFromBacking(\_:) 

Instance Method

# convertFromBacking(\_:)

Converts a rectangle from its pixel-aligned backing store coordinate system to the window’s coordinate system.

macOS 10.7+

``` source
@MainActor
func convertFromBacking(_ rect: NSRect) -> NSRect
```

## Parameters 

`rect`  

The rectangle aligned to the pixel backing store coordinate system.

## Return Value

A rectangle in the window’s coordinate system.

## See Also

### Converting Coordinates

var backingScaleFactor: CGFloat

The backing scale factor.

func backingAlignedRect(NSRect, options: AlignmentOptions) -> NSRect

Returns a backing store pixel-aligned rectangle in window coordinates.

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

