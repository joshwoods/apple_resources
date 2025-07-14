

- SwiftUI
- Shape
-  scale(x:y:anchor:) 

Instance Method

# scale(x:y:anchor:)

Scales this shape without changing its bounding frame.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func scale(
    x: CGFloat = 1,
    y: CGFloat = 1,
    anchor: UnitPoint = .center
) -> ScaledShape
```

## Parameters 

`x`  

The multiplication factor used to resize this shape along its x-axis.

`y`  

The multiplication factor used to resize this shape along its y-axis.

## Return Value

A scaled form of this shape.

## Discussion

Both the `x` and `y` multiplication factors halve their respective dimension’s size when set to `0.5`, maintain their existing size when set to `1`, double their size when set to `2`, and so forth.

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

func rotation(Angle, anchor: UnitPoint) -> RotatedShape&lt;Self>

Rotates this shape around an anchor point at the angle you specify.

func offset(_:)

Changes the relative position of this shape using the specified point.

func offset(x: CGFloat, y: CGFloat) -> OffsetShape&lt;Self>

Changes the relative position of this shape using the specified point.

