

- Spatial
- Ray3D
-  intersects(sphereOrigin:sphereRadius:) 

Instance Method

# intersects(sphereOrigin:sphereRadius:)

Returns a Boolean value that indicates whether the ray intersects a specified sphere.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func intersects(
    sphereOrigin: Point3D,
    sphereRadius: Double
) -> Bool
```

## See Also

### Checking characteristics

var isFinite: Bool

A Boolean value that indicates whether all of the values of the ray are finite.

var isNaN: Bool

A Boolean value that indicates whether the ray contains any NaN values.

var isZero: Bool

A Boolean value that indicates whether all of the values of the ray are zero.

func intersects(Rect3D) -> Bool

Returns a Boolean value that indicates whether a ray intersects a rectangle.

