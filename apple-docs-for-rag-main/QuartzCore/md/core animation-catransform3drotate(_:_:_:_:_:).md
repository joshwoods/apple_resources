

- Core Animation
-  CATransform3DRotate(\_:\_:\_:\_:\_:) 

Function

# CATransform3DRotate(\_:\_:\_:\_:\_:)

Rotates `t` by `angle` radians about the vector `(x, y, z)` and returns the result.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DRotate(
    _ t: CATransform3D,
    _ angle: CGFloat,
    _ x: CGFloat,
    _ y: CGFloat,
    _ z: CGFloat
) -> CATransform3D
```

## Discussion

If the vector has zero length, the behavior is undefined: `t` = `rotation(angle, x, y, z) * t`.

## See Also

### Chaining Transforms

func CATransform3DConcat(CATransform3D, CATransform3D) -> CATransform3D

Concatenates `b` to `a` and returns the result: `t = a * b`.

func CATransform3DTranslate(CATransform3D, CGFloat, CGFloat, CGFloat) -> CATransform3D

Translates `t` by `(tx, ty, tz)` and returns the result: `t` `= translate(tx, ty, tz) * t`.

func CATransform3DScale(CATransform3D, CGFloat, CGFloat, CGFloat) -> CATransform3D

Scales `t` by `(sx, sy, sz)` and returns the result: `t = scale(sx, sy, sz) * t`.

