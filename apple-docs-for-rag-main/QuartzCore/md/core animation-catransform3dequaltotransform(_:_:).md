

- Core Animation
-  CATransform3DEqualToTransform(\_:\_:) 

Function

# CATransform3DEqualToTransform(\_:\_:)

Returns a Boolean value that indicates whether the two transforms are exactly equal.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DEqualToTransform(
    _ a: CATransform3D,
    _ b: CATransform3D
) -> Bool
```

## Return Value

true if `a` and `b` are exactly equal, otherwise false.

## See Also

### Determining Transform Properties

func CATransform3DIsAffine(CATransform3D) -> Bool

Returns a Boolean value that indicates whether a transform can be exactly represented by an affine transform.

func CATransform3DIsIdentity(CATransform3D) -> Bool

Returns a Boolean value that indicates whether the transform is the identity transform.

