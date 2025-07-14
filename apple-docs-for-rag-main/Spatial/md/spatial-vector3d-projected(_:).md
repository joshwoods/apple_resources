

- Spatial
- Vector3D
-  projected(\_:) 

Instance Method

# projected(\_:)

Returns the vector projected onto the specified vector.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func projected(_ other: Vector3D) -> Vector3D
```

## Parameters 

`other`  

The second vector.

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

var normalized: Vector3D

A new vector that represents the normalized copy of the current vector.

func reflected(Vector3D) -> Vector3D

Returns the reflection direction of the incident vector and a specified unit normal vector.

