

- Spatial
- ProjectiveTransform3D
-  concatenating(\_:) 

Instance Method

# concatenating(\_:)

Returns a projective transformation matrix that results from concatenating two existing projective transforms.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func concatenating(_ t2: ProjectiveTransform3D) -> ProjectiveTransform3D
```

## Parameters 

`t2`  

The projective transform that the function concatenates to this projective transform.

## Return Value

The projective transformation matrix that results from concatenating two existing projective transforms.

## Discussion

This function performs the matrix multiplication `self * t2` on the underlying matrices of the two transforms.

## See Also

### Transforming a 3D projective transform structure

func sheared(AxisWithFactors) -> ProjectiveTransform3D

Returns a projective transform that results from shearing over an axis by shear factors for the other two axes.

enum AxisWithFactors

Constants that describe the axis of a shear transform.

struct Axis3D

Constants that describe an axis.

func flip(along: Axis3D)

Flips a projective transform along the specified axis.

func flipped(along: Axis3D) -> ProjectiveTransform3D

Returns a projective transform that results from flipping it along the specified axis.

