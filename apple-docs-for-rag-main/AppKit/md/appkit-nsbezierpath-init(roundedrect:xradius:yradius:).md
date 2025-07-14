

- AppKit
- NSBezierPath
-  init(roundedRect:xRadius:yRadius:) 

Initializer

# init(roundedRect:xRadius:yRadius:)

Creates and returns a new Bézier path object initialized with a rounded rectangular path.

macOS 10.5+

``` source
init(
    roundedRect rect: NSRect,
    xRadius: CGFloat,
    yRadius: CGFloat
)
```

## Parameters 

`rect`  

The rectangle that defines the basic shape of the path.

`xRadius`  

The radius of each corner oval along the x-axis. Values larger than half the rectangle’s width are clamped to half the width.

`yRadius`  

The radius of each corner oval along the y-axis. Values larger than half the rectangle’s height are clamped to half the height.

## Return Value

A new path object with the rounded rectangular path.

## Discussion

The path is constructed in a counter-clockwise direction, starting at the top-left corner of the rectangle. If either one of the radius parameters contains the value `0.0`, the returned path is a plain rectangle without rounded corners.

## See Also

### Related Documentation

func appendRoundedRect(NSRect, xRadius: CGFloat, yRadius: CGFloat)

Appends a rounded rectangular path to the path.

### Creating a Bézier Path

init(ovalIn: NSRect)

Creates and returns a new Bézier path object initialized with an oval path inscribed in the specified rectangle.

init(rect: NSRect)

Creates and returns a new Bézier path object initialized with a rectangular path.

init(cgPath: CGPath)

var flattened: NSBezierPath

A flattened version of the path object.

var reversed: NSBezierPath

A path containing the reversed contents of the current path object.

