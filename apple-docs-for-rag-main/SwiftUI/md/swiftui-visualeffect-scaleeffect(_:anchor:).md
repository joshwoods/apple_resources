

- SwiftUI
- VisualEffect
-  scaleEffect(\_:anchor:) 

Instance Method

# scaleEffect(\_:anchor:)

Scales this view uniformly by the specified factor.

visionOS 1.0+

``` source
func scaleEffect(
    _ s: CGFloat,
    anchor: UnitPoint3D = .center
) -> some VisualEffect
```

Show all declarations

## Parameters 

`s`  

The scale factor for this view.

`anchor`  

The anchor point about which to scale the view. Defaults to center.

## Return Value

An effect that scales this view by `s` in all dimensions.

## Discussion

The original dimensions of the view are considered to be unchanged by scaling the contents. To change the dimensions of the view, use a modifier like `frame()` instead.

## See Also

### Scaling

func scaleEffect(x: CGFloat, y: CGFloat, anchor: UnitPoint) -> some VisualEffect

Scales the view’s rendered output by the given horizontal and vertical amounts, relative to an anchor point.

func scaleEffect(x: CGFloat, y: CGFloat, z: CGFloat, anchor: UnitPoint3D) -> some VisualEffect

Scales this view by the specified horizontal, vertical, and depth factors.

