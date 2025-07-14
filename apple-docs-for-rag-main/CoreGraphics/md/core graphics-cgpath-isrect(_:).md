

- Core Graphics
- CGPath
-  isRect(\_:) 

Instance Method

# isRect(\_:)

Indicates whether or not a graphics path represents a rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func isRect(_ rect: UnsafeMutablePointer?) -> Bool
```

## Parameters 

`rect`  

On input, a pointer to an uninitialized rectangle. If the specified path represents a rectangle, on return contains a copy of the rectangle.

## Return Value

A Boolean value that indicates whether the specified path represents a rectangle. If the path represents a rectangle, returns true.

## See Also

### Examining a Graphics Path

var boundingBox: CGRect

Returns the bounding box containing all points in a graphics path.

var boundingBoxOfPath: CGRect

Returns the bounding box of a graphics path.

var currentPoint: CGPoint

Returns the current point in a graphics path.

func contains(CGPoint, using: CGPathFillRule, transform: CGAffineTransform) -> Bool

Returns whether the specified point is interior to the path.

var isEmpty: Bool

Indicates whether or not a graphics path is empty.

