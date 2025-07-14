

- Core Animation
-  CATransform3DMakeAffineTransform(\_:) 

Function

# CATransform3DMakeAffineTransform(\_:)

Returns a transform with the same effect as affine transform `m`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DMakeAffineTransform(_ m: CGAffineTransform) -> CATransform3D
```

## See Also

### Converting to and from Core Graphics Affine Transforms

func CATransform3DGetAffineTransform(CATransform3D) -> CGAffineTransform

Returns the affine transform represented by `t`.

