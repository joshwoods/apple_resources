

- SwiftUI
- Shape
-  scale(\_:anchor:) 

Instance Method

# scale(\_:anchor:)

Scales this shape without changing its bounding frame.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func scale(
    _ scale: CGFloat,
    anchor: UnitPoint = .center
) -> ScaledShape
```

## Parameters 

`scale`  

The multiplication factor used to resize this shape. A value of `0` scales the shape to have no size, `0.5` scales to half size in both dimensions, `2` scales to twice the regular size, and so on.

## Return Value

A scaled form of this shape.

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

func scale(x: CGFloat, y: CGFloat, anchor: UnitPoint) -> ScaledShape&lt;Self>

Scales this shape without changing its bounding frame.

func rotation(Angle, anchor: UnitPoint) -> RotatedShape&lt;Self>

Rotates this shape around an anchor point at the angle you specify.

func offset(_:)

Changes the relative position of this shape using the specified point.

func offset(x: CGFloat, y: CGFloat) -> OffsetShape&lt;Self>

Changes the relative position of this shape using the specified point.

