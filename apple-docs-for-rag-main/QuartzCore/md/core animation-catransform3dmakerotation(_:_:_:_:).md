

- Core Animation
-  CATransform3DMakeRotation(\_:\_:\_:\_:) 

Function

# CATransform3DMakeRotation(\_:\_:\_:\_:)

Returns a transform that rotates by `angle` radians about the vector `(x, y, z)`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DMakeRotation(
    _ angle: CGFloat,
    _ x: CGFloat,
    _ y: CGFloat,
    _ z: CGFloat
) -> CATransform3D
```

## Discussion

If the vector has length zero, this function returns the identity transform.

## See Also

### Creating Transforms

func CATransform3DMakeTranslation(CGFloat, CGFloat, CGFloat) -> CATransform3D

Returns a transform that translates by `(tx, ty, tz)`.

func CATransform3DMakeScale(CGFloat, CGFloat, CGFloat) -> CATransform3D

Returns a transform that scales by `(sx, sy, sz)`.

