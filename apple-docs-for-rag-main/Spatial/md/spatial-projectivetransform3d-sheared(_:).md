

- Spatial
- ProjectiveTransform3D
-  sheared(\_:) 

Instance Method

# sheared(\_:)

Returns a projective transform that results from shearing over an axis by shear factors for the other two axes.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func sheared(_ shear: AxisWithFactors) -> ProjectiveTransform3D
```

## Parameters 

`shear`  

The shear axis and factors.

## Return Value

The projective transform that results from shearing over an axis by shear factors for the other two axes.

## See Also

### Transforming a 3D projective transform structure

enum AxisWithFactors

Constants that describe the axis of a shear transform.

struct Axis3D

Constants that describe an axis.

func concatenating(ProjectiveTransform3D) -> ProjectiveTransform3D

Returns a projective transformation matrix that results from concatenating two existing projective transforms.

func flip(along: Axis3D)

Flips a projective transform along the specified axis.

func flipped(along: Axis3D) -> ProjectiveTransform3D

Returns a projective transform that results from flipping it along the specified axis.

