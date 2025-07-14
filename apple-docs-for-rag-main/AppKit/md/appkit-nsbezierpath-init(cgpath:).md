

- AppKit
- NSBezierPath
-  init(cgPath:) 

Initializer

# init(cgPath:)

macOS 14.0+

``` source
init(cgPath: CGPath)
```

## See Also

### Creating a Bézier Path

init(ovalIn: NSRect)

Creates and returns a new Bézier path object initialized with an oval path inscribed in the specified rectangle.

init(rect: NSRect)

Creates and returns a new Bézier path object initialized with a rectangular path.

init(roundedRect: NSRect, xRadius: CGFloat, yRadius: CGFloat)

Creates and returns a new Bézier path object initialized with a rounded rectangular path.

var flattened: NSBezierPath

A flattened version of the path object.

var reversed: NSBezierPath

A path containing the reversed contents of the current path object.

