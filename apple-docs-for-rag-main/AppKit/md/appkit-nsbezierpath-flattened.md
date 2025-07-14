

- AppKit
- NSBezierPath
-  flattened 

Instance Property

# flattened

A flattened version of the path object.

macOS

``` source
@NSCopying
var flattened: NSBezierPath { get }
```

## Discussion

Flattening a path converts all curved line segments into straight line approximations. The granularity of the approximations is controlled by the path’s current flatness value, which is set using defaultFlatness.

## See Also

### Creating a Bézier Path

init(ovalIn: NSRect)

Creates and returns a new Bézier path object initialized with an oval path inscribed in the specified rectangle.

init(rect: NSRect)

Creates and returns a new Bézier path object initialized with a rectangular path.

init(roundedRect: NSRect, xRadius: CGFloat, yRadius: CGFloat)

Creates and returns a new Bézier path object initialized with a rounded rectangular path.

init(cgPath: CGPath)

var reversed: NSBezierPath

A path containing the reversed contents of the current path object.

