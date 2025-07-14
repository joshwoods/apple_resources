

- SwiftUI
- HoverEffectContent
-  rotationEffect(\_:anchor:) 

Instance Method

# rotationEffect(\_:anchor:)

Rotates content in two dimensions around the specified point.

visionOS 2.0+

``` source
func rotationEffect(
    _ angle: Angle,
    anchor: UnitPoint = .center
) -> some HoverEffectContent
```

## Parameters 

`angle`  

The angle by which to rotate the content.

`anchor`  

A unit point within the content about which to perform the rotation. The default value is center.

## Return Value

A rotation effect.

## Discussion

This effect rotates the content around the axis that points out of the xy-plane. It has no effect on the content’s frame.

