

- Vision
- VNVector
-  init(r:theta:) 

Initializer

# init(r:theta:)

Creates a new vector in polar coordinate space.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
convenience init(
    r: Double,
    theta: Double
)
```

## Parameters 

`r`  

The length of the vector.

`theta`  

The angle that the vector forms with the positive direction of the x-axis.

## See Also

### Creating a Vector

init(byAdding: VNVector, to: VNVector)

Creates a new vector by adding the specified vectors.

init(bySubtracting: VNVector, from: VNVector)

Creates a new vector by subtracting the first vector from the second vector.

init(byMultiplying: VNVector, byScalar: Double)

Creates a new vector by multiplying the specified vector’s x-axis and y-axis projections by the scalar value.

convenience init(vectorHead: VNPoint, tail: VNPoint)

Creates a new vector in Cartesian coordinate space.

init(xComponent: Double, yComponent: Double)

Creates a new vector in Cartesian coordinate space, based on its x-axis and y-axis projections.

class var zero: VNVector

A vector object with zero length.

