

- Core Graphics
- CGPath
-  contains(\_:using:transform:) 

Instance Method

# contains(\_:using:transform:)

Returns whether the specified point is interior to the path.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(
    _ point: CGPoint,
    using rule: CGPathFillRule = .winding,
    transform: CGAffineTransform = .identity
) -> Bool
```

## Parameters 

`point`  

The point to check.

`rule`  

The rule for determining which areas to treat as the interior of the path. Defaults to the CGPathFillRule.winding rule if not specified.

`transform`  

An affine transform to apply to the point before checking for containment in the path. Defaults to the CGAffineTransformIdentity transform if not specified.

## Return Value

true if the point is interior to the path; otherwise, false.

## Discussion

A point is contained in a path if it would be inside the painted region when the path is filled.

## See Also

### Related Documentation

enum CGPathFillRule

Rules for determining which regions are interior to a path, used by the fillPath(using:) and clip(using:) methods.

### Examining a Graphics Path

var boundingBox: CGRect

Returns the bounding box containing all points in a graphics path.

var boundingBoxOfPath: CGRect

Returns the bounding box of a graphics path.

var currentPoint: CGPoint

Returns the current point in a graphics path.

var isEmpty: Bool

Indicates whether or not a graphics path is empty.

func isRect(UnsafeMutablePointer&lt;CGRect>?) -> Bool

Indicates whether or not a graphics path represents a rectangle.

