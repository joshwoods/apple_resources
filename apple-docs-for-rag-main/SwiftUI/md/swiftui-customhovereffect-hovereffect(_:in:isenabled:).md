

- SwiftUI
- CustomHoverEffect
-  hoverEffect(\_:in:isEnabled:) 

Instance Method

# hoverEffect(\_:in:isEnabled:)

Applies this effect in parallel with the given `effect`.

visionOS 2.0+

``` source
func hoverEffect(
    _ effect: some CustomHoverEffect,
    in group: HoverEffectGroup? = nil,
    isEnabled: Bool = true
) -> some CustomHoverEffect
```

## Parameters 

`effect`  

A CustomHoverEffect to combine with this effect.

`group`  

An optional HoverEffectGroup to add this effect to.

`isEnabled`  

Whether `effect` is enabled or not.

## Discussion

Use `hoverEffect(_:)` to combine two effects into a single effect that applies both effects in parallel. Modifiers like hoverEffectDisabled(_:) applied to `effect` will not apply to this effect.

For example, in the following effect only the `ScaleUpEffect` will be disabled, since modifiers applied to that effect will applied independently.

```
struct FadeAndScaleEffect: CustomHoverEffect {
    @Environment(\.accessibilityReduceMotion) var accessibilityReduceMotion
    func body(content: Content) -> some CustomHoverEffect {
        content
            .hoverEffect { effect, isActive, _ in
                effect.opacity(isActive ? 1 : 0.9)
            }
            .hoverEffect(
                ScaleUpEffect().hoverEffectDisabled(accessibilityReduceMotion)
            )
    }
}

struct ScaleUpEffect: CustomHoverEffect {
    func body(content: Content) -> some CustomHoverEffect {
        content.hoverEffect { effect, isActive, _ in
            effect.scaleEffect(isActive ? 1.05 : 1.0)
        }
    }
}
```

- Returns a new effect that applies both effects in parallel.

## See Also

### Creating custom hover effects

func hoverEffect(in: HoverEffectGroup?, isEnabled: Bool, body: (EmptyHoverEffectContent, Bool, GeometryProxy) -> some HoverEffectContent) -> some CustomHoverEffect

Applies a hover effect based on the current phase.

func hoverEffectGroup(HoverEffectGroup?) -> some CustomHoverEffect

Activates this effect as part of an effect group.

func hoverEffectGroup(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior) -> some CustomHoverEffect

Activates this effect as part of an effect group.

func hoverEffectDisabled(Bool) -> some CustomHoverEffect

Disables this hover effect.

