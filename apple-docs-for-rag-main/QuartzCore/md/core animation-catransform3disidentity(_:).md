

- Core Animation
-  CATransform3DIsIdentity(\_:) 

Function

# CATransform3DIsIdentity(\_:)

Returns a Boolean value that indicates whether the transform is the identity transform.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DIsIdentity(_ t: CATransform3D) -> Bool
```

## Return Value

true if `t` is the identity transform, otherwise false.

## See Also

### Determining Transform Properties

func CATransform3DIsAffine(CATransform3D) -> Bool

Returns a Boolean value that indicates whether a transform can be exactly represented by an affine transform.

func CATransform3DEqualToTransform(CATransform3D, CATransform3D) -> Bool

Returns a Boolean value that indicates whether the two transforms are exactly equal.

