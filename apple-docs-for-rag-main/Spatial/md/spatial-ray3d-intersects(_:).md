

- Spatial
- Ray3D
-  intersects(\_:) 

Instance Method

# intersects(\_:)

Returns a Boolean value that indicates whether a ray intersects a rectangle.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func intersects(_ rect: Rect3D) -> Bool
```

## Parameters 

`rect`  

The rectangle that the function compares against.

## Return Value

A Boolean value that indicates whether the ray intersects the rectangle.

## See Also

### Checking characteristics

var isFinite: Bool

A Boolean value that indicates whether all of the values of the ray are finite.

var isNaN: Bool

A Boolean value that indicates whether the ray contains any NaN values.

var isZero: Bool

A Boolean value that indicates whether all of the values of the ray are zero.

func intersects(sphereOrigin: Point3D, sphereRadius: Double) -> Bool

Returns a Boolean value that indicates whether the ray intersects a specified sphere.

