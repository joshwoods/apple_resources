

- AppKit
- NSBezierPath
-  init(rect:) 

Initializer

# init(rect:)

Creates and returns a new Bézier path object initialized with a rectangular path.

macOS

``` source
init(rect: NSRect)
```

## Parameters 

`rect`  

The rectangle describing the path to create.

## Return Value

A new path object with the rectangular path.

## Discussion

The path is constructed by starting at the origin of `aRect` and adding line segments in a counterclockwise direction.

## See Also

### Related Documentation

class func fill(NSRect)

Fills the specified rectangular path with the current fill color.

class func stroke(NSRect)

Strokes the path of the specified rectangle using the current stroke color and the default drawing attributes.

func appendRect(NSRect)

Appends a rectangular path to the path.

### Creating a Bézier Path

init(ovalIn: NSRect)

Creates and returns a new Bézier path object initialized with an oval path inscribed in the specified rectangle.

init(roundedRect: NSRect, xRadius: CGFloat, yRadius: CGFloat)

Creates and returns a new Bézier path object initialized with a rounded rectangular path.

init(cgPath: CGPath)

var flattened: NSBezierPath

A flattened version of the path object.

var reversed: NSBezierPath

A path containing the reversed contents of the current path object.

