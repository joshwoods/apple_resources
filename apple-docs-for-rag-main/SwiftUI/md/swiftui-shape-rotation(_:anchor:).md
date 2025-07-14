

- SwiftUI
- Shape
-  rotation(\_:anchor:) 

Instance Method

# rotation(\_:anchor:)

Rotates this shape around an anchor point at the angle you specify.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func rotation(
    _ angle: Angle,
    anchor: UnitPoint = .center
) -> RotatedShape
```

## Parameters 

`angle`  

The angle of rotation to apply. Positive angles rotate clockwise; negative angles rotate counterclockwise.

`anchor`  

The point to rotate the shape around.

## Return Value

A rotated shape.

## Discussion

The following example rotates a square by 45 degrees to the right to create a diamond shape:

```
RoundedRectangle(cornerRadius: 10)
.rotation(Angle(degrees: 45))
.aspectRatio(1.0, contentMode: .fit)
```

## See Also

### Transforming a shape

func trim(from: CGFloat, to: CGFloat) -> some Shape

Trims this shape by a fractional amount based on its representation as a path.

func transform(CGAffineTransform) -> TransformedShape&lt;Self>

Applies an affine transform to this shape.

func size(CGSize) -> some Shape

Returns a new version of self representing the same shape, but that will ask it to create its path from a rect of `size`. This does not affect the layout properties of any views created from the shape (e.g. by filling it).

func size(width: CGFloat, height: CGFloat) -> some Shape

Returns a new version of self representing the same shape, but that will ask it to create its path from a rect of size `(width, height)`. This does not affect the layout properties of any views created from the shape (e.g. by filling it).

func scale(CGFloat, anchor: UnitPoint) -> ScaledShape&lt;Self>

Scales this shape without changing its bounding frame.

func scale(x: CGFloat, y: CGFloat, anchor: UnitPoint) -> ScaledShape&lt;Self>

Scales this shape without changing its bounding frame.

func offset(_:)

Changes the relative position of this shape using the specified point.

func offset(x: CGFloat, y: CGFloat) -> OffsetShape&lt;Self>

Changes the relative position of this shape using the specified point.

