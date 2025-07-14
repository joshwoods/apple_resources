

- Spatial
- Rect3D
-  contains(anyOf:) 

Instance Method

# contains(anyOf:)

Returns a Boolean value that indicates whether the rectangle contains any of the specified points.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func contains(anyOf points: [Point3D]) -> Bool
```

## Parameters 

`points`  

The array of points that the function compares against.

## Return Value

A Boolean value that indicates whether the rectangle contains any of the specified points.

## See Also

### Checking characteristics

func intersects(Rect3D) -> Bool

Returns a Boolean value that indicates whether two rectangles intersect.

var isEmpty: Bool

A Boolean value that indicates whether two or three of the dimensions are zero.

