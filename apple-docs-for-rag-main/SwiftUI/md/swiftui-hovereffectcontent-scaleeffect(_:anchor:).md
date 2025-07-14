

- SwiftUI
- HoverEffectContent
-  scaleEffect(\_:anchor:) 

Instance Method

# scaleEffect(\_:anchor:)

Scales the view’s rendered output by the given amount in both the horizontal and vertical directions, relative to an anchor point.

visionOS 2.0+

``` source
func scaleEffect(
    _ scale: CGFloat,
    anchor: UnitPoint = .center
) -> some HoverEffectContent
```

Show all declarations

## Parameters 

`scale`  

The amount to scale the view in the view in both the horizontal and vertical directions.

`anchor`  

The point with a default of center that defines the location within the view from which to apply the transformation.

## Return Value

An effect that scales the view’s rendered output.

