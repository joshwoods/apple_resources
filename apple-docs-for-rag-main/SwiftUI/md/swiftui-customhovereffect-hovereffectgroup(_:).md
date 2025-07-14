

- SwiftUI
- CustomHoverEffect
-  hoverEffectGroup(\_:) 

Instance Method

# hoverEffectGroup(\_:)

Activates this effect as part of an effect group.

visionOS 2.0+

``` source
func hoverEffectGroup(_ group: HoverEffectGroup?) -> some CustomHoverEffect
```

## Parameters 

`group`  

The `HoverEffectGroup` to activate when this view is hovered. If `nil`, this modifier has no effect.

## Return Value

A view that activates the given hover group.

## Discussion

You use this method to compose effects that affect multiple views in concert. In the following example, both views’ effects are in the same group. As a result, hovering over either view will activate all effects in the group, causing both views to become fully opaque:

```
struct EffectView: View {
    var effectGroup: HoverEffectGroup?

    var body: some View {
        Color.red
            .frame(width: 100, height: 100)
            .hoverEffect(
                FadeEffect().hoverEffectGroup(effectGroup)
            )
        Color.blue
            .frame(width: 100, height: 100)
            .hoverEffect(
                FadeEffect().hoverEffectGroup(effectGroup)
            )
    }
}

struct FadeEffect: CustomHoverEffect {
    func body(content: Content) -> some CustomHoverEffect {
        content.hoverEffect { effect, isActive, _ in
            effect.opacity(isActive ? 1 : 0.5)
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

func hoverEffectGroup(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior) -> some CustomHoverEffect

Activates this effect as part of an effect group.

func hoverEffectDisabled(Bool) -> some CustomHoverEffect

Disables this hover effect.

