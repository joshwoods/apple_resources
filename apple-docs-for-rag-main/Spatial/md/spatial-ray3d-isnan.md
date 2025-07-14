

- Spatial
- Ray3D
-  isNaN 

Instance Property

# isNaN

A Boolean value that indicates whether the ray contains any NaN values.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var isNaN: Bool { get }
```

## See Also

### Checking characteristics

var isFinite: Bool

A Boolean value that indicates whether all of the values of the ray are finite.

var isZero: Bool

A Boolean value that indicates whether all of the values of the ray are zero.

func intersects(Rect3D) -> Bool

Returns a Boolean value that indicates whether a ray intersects a rectangle.

func intersects(sphereOrigin: Point3D, sphereRadius: Double) -> Bool

Returns a Boolean value that indicates whether the ray intersects a specified sphere.

