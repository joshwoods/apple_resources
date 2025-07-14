

- Core Animation
-  CATransform3DMakeScale(\_:\_:\_:) 

Function

# CATransform3DMakeScale(\_:\_:\_:)

Returns a transform that scales by `(sx, sy, sz)`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DMakeScale(
    _ sx: CGFloat,
    _ sy: CGFloat,
    _ sz: CGFloat
) -> CATransform3D
```

## Discussion

`t = [sx 0 0 0; 0 sy 0 0; 0 0 sz 0; 0 0 0 1].`

## See Also

### Creating Transforms

func CATransform3DMakeTranslation(CGFloat, CGFloat, CGFloat) -> CATransform3D

Returns a transform that translates by `(tx, ty, tz)`.

func CATransform3DMakeRotation(CGFloat, CGFloat, CGFloat, CGFloat) -> CATransform3D

Returns a transform that rotates by `angle` radians about the vector `(x, y, z)`.

