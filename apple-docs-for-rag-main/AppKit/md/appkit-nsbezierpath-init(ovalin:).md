

- AppKit
- NSBezierPath
-  init(ovalIn:) 

Initializer

# init(ovalIn:)

Creates and returns a new Bézier path object initialized with an oval path inscribed in the specified rectangle.

macOS

``` source
init(ovalIn rect: NSRect)
```

## Parameters 

`rect`  

The rectangle in which to inscribe an oval.

## Return Value

An `NSBezierPath` new path object with the oval path.

## Discussion

If the `aRect` parameter specifies a square, the inscribed path is a circle. The path is constructed by starting in the lower-right quadrant of the rectangle and adding arc segments counterclockwise to complete the oval.

## See Also

### Related Documentation

func appendOval(in: NSRect)

Appends an oval path to the path, inscribing the oval in the specified rectangle.

### Creating a Bézier Path

init(rect: NSRect)

Creates and returns a new Bézier path object initialized with a rectangular path.

init(roundedRect: NSRect, xRadius: CGFloat, yRadius: CGFloat)

Creates and returns a new Bézier path object initialized with a rounded rectangular path.

init(cgPath: CGPath)

var flattened: NSBezierPath

A flattened version of the path object.

var reversed: NSBezierPath

A path containing the reversed contents of the current path object.

