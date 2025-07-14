

- Core Animation
-  CATransform3DMakeTranslation(\_:\_:\_:) 

Function

# CATransform3DMakeTranslation(\_:\_:\_:)

Returns a transform that translates by `(tx, ty, tz)`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DMakeTranslation(
    _ tx: CGFloat,
    _ ty: CGFloat,
    _ tz: CGFloat
) -> CATransform3D
```

## Discussion

`t = [1 0 0 0; 0 1 0 0; 0 0 1 0; tx ty tz 1].`

## See Also

### Creating Transforms

func CATransform3DMakeScale(CGFloat, CGFloat, CGFloat) -> CATransform3D

Returns a transform that scales by `(sx, sy, sz)`.

func CATransform3DMakeRotation(CGFloat, CGFloat, CGFloat, CGFloat) -> CATransform3D

Returns a transform that rotates by `angle` radians about the vector `(x, y, z)`.

