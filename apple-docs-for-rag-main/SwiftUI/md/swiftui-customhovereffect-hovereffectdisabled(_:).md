

- SwiftUI
- CustomHoverEffect
-  hoverEffectDisabled(\_:) 

Instance Method

# hoverEffectDisabled(\_:)

Disables this hover effect.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
func hoverEffectDisabled(_ isDisabled: Bool = true) -> some CustomHoverEffect
```

## Parameters 

`isDisabled`  

A Boolean value that determines whether the hover effect is disabled or not. Specifying `true` takes precedence over `false`. Default: `true`.

## Return Value

A conditionally disabled hover effect.

## Discussion

Use `hoverEffectDisabled(_:)` to prevent a hover effect from becoming active. When an effect is disabled, all contained effects are also disabled and cannot be re-enabled.

In the following example, the scale effect is disabled if the `accessibilityReduceMotion` setting is enabled:

```
struct ScaleAndFadeEffect: CustomHoverEffect {
    @Environment(\.accessibilityReduceMotion) var accessibilityReduceMotion
    func body(content: Content) -> some CustomHoverEffect {
        content.hoverEffect { effect, isActive, _ in
            effect.scaleEffect(!isActive ? 0.95 : 1.05)
        }
        .hoverEffectDisabled(accessibilityReduceMotion)
        .hoverEffect { effect, isActive, _ in
            effect.opacity(!isActive ? 0.9 : 1)
        }
    }
}
```

## See Also

### Creating custom hover effects

func hoverEffect(some CustomHoverEffect, in: HoverEffectGroup?, isEnabled: Bool) -> some CustomHoverEffect

Applies this effect in parallel with the given `effect`.

func hoverEffect(in: HoverEffectGroup?, isEnabled: Bool, body: (EmptyHoverEffectContent, Bool, GeometryProxy) -> some HoverEffectContent) -> some CustomHoverEffect

Applies a hover effect based on the current phase.

func hoverEffectGroup(HoverEffectGroup?) -> some CustomHoverEffect

Activates this effect as part of an effect group.

func hoverEffectGroup(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior) -> some CustomHoverEffect

Activates this effect as part of an effect group.

