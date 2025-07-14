

- Core Graphics
- CGContext
-  currentPointOfPath 

Instance Property

# currentPointOfPath

Returns the current point in a non-empty path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var currentPointOfPath: CGPoint { get }
```

## See Also

### Examining the Current Graphics Path

var boundingBoxOfPath: CGRect

Returns the smallest rectangle that contains the current path.

var isPathEmpty: Bool

Indicates whether the current path contains any subpaths.

func pathContains(CGPoint, mode: CGPathDrawingMode) -> Bool

Checks to see whether the specified point is contained in the current path.

