

- AppKit
- NSWindow
-  convertPointFromBacking(\_:) 

Instance Method

# convertPointFromBacking(\_:)

Converts a point from its pixel-aligned backing store coordinate system to the window’s coordinate system.

macOS 10.14+

``` source
@MainActor
func convertPointFromBacking(_ point: NSPoint) -> NSPoint
```

## Parameters 

`point`  

The point in the pixel-aligned backing store coordinate system.

## Return Value

A point in the window’s coordinate system.

## See Also

### Converting Coordinates

var backingScaleFactor: CGFloat

The backing scale factor.

func backingAlignedRect(NSRect, options: AlignmentOptions) -> NSRect

Returns a backing store pixel-aligned rectangle in window coordinates.

func convertFromBacking(NSRect) -> NSRect

Converts a rectangle from its pixel-aligned backing store coordinate system to the window’s coordinate system.

func convertFromScreen(NSRect) -> NSRect

Converts a rectangle from the screen coordinate system to the window’s coordinate system.

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

