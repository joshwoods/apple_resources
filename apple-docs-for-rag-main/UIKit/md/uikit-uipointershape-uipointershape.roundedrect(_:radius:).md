

- UIKit
- UIPointerShape
-  UIPointerShape.roundedRect(\_:radius:) 

Case

# UIPointerShape.roundedRect(\_:radius:)

The pointer morphs into a rounded rectangle using the provided corner radius.

iOS 13.4+iPadOS 13.4+Mac CatalystvisionOS

``` source
case roundedRect(
    CGRect,
    radius: CGFloat = UIPointerShape.defaultCornerRadius
)
```

## Discussion

If you don’t specify a radius, the rounded rectangle uses the `defaultCornerRadius`.

Note

If used alongside a content effect, this rectangle must be in the view coordinate space of the preview. Otherwise, it’s centered around the pointer’s current location, and the rectangle’s origin is interpreted as an offset.

## See Also

### Specifying pointer shapes

case horizontalBeam(length: CGFloat)

The pointer morphs into a horizontal beam using the specified length.

case verticalBeam(length: CGFloat)

The pointer morphs into a vertical beam using the specified length.

case path(UIBezierPath)

The pointer morphs into the given Bézier path.

