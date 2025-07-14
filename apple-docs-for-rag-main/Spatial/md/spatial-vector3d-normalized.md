

- Spatial
- Vector3D
-  normalized 

Instance Property

# normalized

A new vector that represents the normalized copy of the current vector.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
var normalized: Vector3D { get }
```

## See Also

### Geometry functions

func cross(Vector3D) -> Vector3D

Returns the cross product of the vector and the specified vector.

func dot(Vector3D) -> Double

Returns the dot product of the vector and the specified vector.

var length: Double

The length of the vector.

var lengthSquared: Double

The square of the length of the vector.

func normalize()

Normalizes the mutable vector.

func projected(Vector3D) -> Vector3D

Returns the vector projected onto the specified vector.

func reflected(Vector3D) -> Vector3D

Returns the reflection direction of the incident vector and a specified unit normal vector.

