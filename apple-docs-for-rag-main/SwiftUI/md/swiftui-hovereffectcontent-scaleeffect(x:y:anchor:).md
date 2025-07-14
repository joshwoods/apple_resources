

- SwiftUI
- HoverEffectContent
-  scaleEffect(x:y:anchor:) 

Instance Method

# scaleEffect(x:y:anchor:)

Scales the view’s rendered output by the given horizontal and vertical amounts, relative to an anchor point.

visionOS 2.0+

``` source
func scaleEffect(
    x: CGFloat = 1.0,
    y: CGFloat = 1.0,
    anchor: UnitPoint = .center
) -> some HoverEffectContent
```

## Parameters 

`x`  

An amount that represents the horizontal amount to scale the view. The default value is `1.0`.

`y`  

An amount that represents the vertical amount to scale the view. The default value is `1.0`.

`anchor`  

The point with a default of center that defines the location within the view from which to apply the transformation.

## Return Value

An effect that scales the view’s rendered output.

