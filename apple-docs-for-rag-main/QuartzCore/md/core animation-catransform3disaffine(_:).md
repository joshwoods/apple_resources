

- Core Animation
-  CATransform3DIsAffine(\_:) 

Function

# CATransform3DIsAffine(\_:)

Returns a Boolean value that indicates whether a transform can be exactly represented by an affine transform.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DIsAffine(_ t: CATransform3D) -> Bool
```

## Discussion

Returns true if `t` can be exactly represented by an affine transform.

## See Also

### Determining Transform Properties

func CATransform3DIsIdentity(CATransform3D) -> Bool

Returns a Boolean value that indicates whether the transform is the identity transform.

func CATransform3DEqualToTransform(CATransform3D, CATransform3D) -> Bool

Returns a Boolean value that indicates whether the two transforms are exactly equal.

