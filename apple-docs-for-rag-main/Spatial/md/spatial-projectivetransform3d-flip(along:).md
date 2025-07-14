

- Spatial
- ProjectiveTransform3D
-  flip(along:) 

Instance Method

# flip(along:)

Flips a projective transform along the specified axis.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func flip(along axis: Axis3D)
```

## Parameters 

`axis`  

An axis structure that specifies the flip axis.

## See Also

### Transforming a 3D projective transform structure

func sheared(AxisWithFactors) -> ProjectiveTransform3D

Returns a projective transform that results from shearing over an axis by shear factors for the other two axes.

enum AxisWithFactors

Constants that describe the axis of a shear transform.

struct Axis3D

Constants that describe an axis.

func concatenating(ProjectiveTransform3D) -> ProjectiveTransform3D

Returns a projective transformation matrix that results from concatenating two existing projective transforms.

func flipped(along: Axis3D) -> ProjectiveTransform3D

Returns a projective transform that results from flipping it along the specified axis.

