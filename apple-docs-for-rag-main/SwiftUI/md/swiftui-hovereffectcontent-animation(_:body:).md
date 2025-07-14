

- SwiftUI
- HoverEffectContent
-  animation(\_:body:) 

Instance Method

# animation(\_:body:)

Applies the given Animation to all effects within the `body` closure.

visionOS 2.0+

``` source
func animation(
    _ animation: Animation?,
    body: (EmptyHoverEffectContent) -> some HoverEffectContent
) -> some HoverEffectContent
```

## Parameters 

`animation`  

The animation to use for the effect transition. If `nil` the effects will not animate.

`body`  

A block used to specify the effects to animate. You must use the provided content to build the effects, or behavior is undefined.

## Return Value

A new effect that combines the effects defined in `body` with

## Discussion

Any effects defined within the `body` closure will be combined with this effect, and the `animation` will used to animate those effects’ changes when the effects are applied.

In the following example, the view will use the `.easeIn` animation when activating the effect, but `.easeOut` when the effect becomes inactive:

```
Color.red
    .hoverEffect { effect, isActive, proxy in
        effect.animation(isActive ? .easeIn : .easeOut) {
            $0.opacity(isActive ? 1 : 0.5)
        }
    }
```

