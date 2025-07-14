

- Core Graphics
- CGContext
-  pathContains(\_:mode:) 

Instance Method

# pathContains(\_:mode:)

Checks to see whether the specified point is contained in the current path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func pathContains(
    _ point: CGPoint,
    mode: CGPathDrawingMode
) -> Bool
```

## Parameters 

`point`  

The point to check, specified in user space units.

`mode`  

A path drawing mode. See CGPathDrawingMode.

## Return Value

Returns `true` if `point` is inside the current path of the graphics context; `false` otherwise.

## Discussion

A point is contained within the path of a graphics context if the point is inside the painted region when the path is stroked or filled with opaque colors using the specified path drawing mode. A point can be inside a path only if the path is explicitly closed by calling the function closePath() for paths drawn directly to the current context, or closeSubpath() for paths first created as CGPath objects and then drawn to the current context.

## See Also

### Examining the Current Graphics Path

var boundingBoxOfPath: CGRect

Returns the smallest rectangle that contains the current path.

var currentPointOfPath: CGPoint

Returns the current point in a non-empty path.

var isPathEmpty: Bool

Indicates whether the current path contains any subpaths.

