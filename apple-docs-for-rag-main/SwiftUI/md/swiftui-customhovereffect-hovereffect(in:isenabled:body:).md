

- SwiftUI
- CustomHoverEffect
-  hoverEffect(in:isEnabled:body:) 

Instance Method

# hoverEffect(in:isEnabled:body:)

Applies a hover effect based on the current phase.

visionOS 2.0+

``` source
func hoverEffect(
    in group: HoverEffectGroup? = nil,
    isEnabled: Bool = true,
    body: @escaping (EmptyHoverEffectContent, Bool, GeometryProxy) -> some HoverEffectContent
) -> some CustomHoverEffect
```

## Parameters 

`group`  

An optional HoverEffectGroup to add this effect to.

`isEnabled`  

Whether the effect is enabled or not. If `false`, the effect’s inactive state will be applied, and it will not apply the active state when hovered.

`body`  

The closure that constructs a `HoverEffectContent` for each of the effect’s phases.

## Return Value

A new effect that changes a view’s appearance when hovered.

## Discussion

You use this modifier to describe how a view should change when hovered. The given closure is provided an empty effect that you use to compose an effect, as well as a boolean describing which phase is being requested. A GeometryProxy is also provided, allowing effects to change based on the view’s geometry.

In the following example, the effect will apply a scale of 1.0 to a view when inactive, and then scale to 1.1 when active:

```
struct ScaleHoverEffect: CustomHoverEffect {
    func body(content: Content) -> some CustomHoverEffect {
        content.hoverEffect { effect, isActive, proxy in
            effect.scaleEffect(!isActive ? 1.0 : 1.1)
        }
    }
}
```

Use the animation(_:body:) modifier to specify how visual changes should be animated.

## See Also

### Creating custom hover effects

func hoverEffect(some CustomHoverEffect, in: HoverEffectGroup?, isEnabled: Bool) -> some CustomHoverEffect

Applies this effect in parallel with the given `effect`.

func hoverEffectGroup(HoverEffectGroup?) -> some CustomHoverEffect

Activates this effect as part of an effect group.

func hoverEffectGroup(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior) -> some CustomHoverEffect

Activates this effect as part of an effect group.

func hoverEffectDisabled(Bool) -> some CustomHoverEffect

Disables this hover effect.

