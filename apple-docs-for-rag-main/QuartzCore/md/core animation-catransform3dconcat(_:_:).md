

- Core Animation
-  CATransform3DConcat(\_:\_:) 

Function

# CATransform3DConcat(\_:\_:)

Concatenates `b` to `a` and returns the result: `t = a * b`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DConcat(
    _ a: CATransform3D,
    _ b: CATransform3D
) -> CATransform3D
```

## See Also

### Chaining Transforms

func CATransform3DTranslate(CATransform3D, CGFloat, CGFloat, CGFloat) -> CATransform3D

Translates `t` by `(tx, ty, tz)` and returns the result: `t` `= translate(tx, ty, tz) * t`.

func CATransform3DScale(CATransform3D, CGFloat, CGFloat, CGFloat) -> CATransform3D

Scales `t` by `(sx, sy, sz)` and returns the result: `t = scale(sx, sy, sz) * t`.

func CATransform3DRotate(CATransform3D, CGFloat, CGFloat, CGFloat, CGFloat) -> CATransform3D

Rotates `t` by `angle` radians about the vector `(x, y, z)` and returns the result.

