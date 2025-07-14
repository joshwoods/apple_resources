

- Core Animation
-  CATransform3DGetAffineTransform(\_:) 

Function

# CATransform3DGetAffineTransform(\_:)

Returns the affine transform represented by `t`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DGetAffineTransform(_ t: CATransform3D) -> CGAffineTransform
```

## Discussion

If `t` can not be exactly represented as an affine transform, the return value is undefined.

## See Also

### Converting to and from Core Graphics Affine Transforms

func CATransform3DMakeAffineTransform(CGAffineTransform) -> CATransform3D

Returns a transform with the same effect as affine transform `m`.

