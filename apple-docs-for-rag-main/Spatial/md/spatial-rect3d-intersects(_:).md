

- Spatial
- Rect3D
-  intersects(\_:) 

Instance Method

# intersects(\_:)

Returns a Boolean value that indicates whether two rectangles intersect.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func intersects(_ other: Rect3D) -> Bool
```

## Parameters 

`other`  

The rectangle that the function compares against.

## Return Value

A Boolean value that indicates whether two rectangles intersect.

## See Also

### Checking characteristics

func contains(anyOf: [Point3D]) -> Bool

Returns a Boolean value that indicates whether the rectangle contains any of the specified points.

var isEmpty: Bool

A Boolean value that indicates whether two or three of the dimensions are zero.

