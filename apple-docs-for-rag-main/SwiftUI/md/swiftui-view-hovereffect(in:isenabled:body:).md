

- SwiftUI
- View
-  hoverEffect(in:isEnabled:body:) 

Instance Method

# hoverEffect(in:isEnabled:body:)

Applies a hover effect to this view described by the given closure.

visionOS 2.0+

``` source
nonisolated
func hoverEffect(
    in group: HoverEffectGroup? = nil,
    isEnabled: Bool = true,
    body: @escaping (EmptyHoverEffectContent, Bool, GeometryProxy) -> some HoverEffectContent
) -> some View
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

You use this modifier to describe how a view should change when hovered. The given block is provided an empty effect that you use to compose effects, as well as a boolean describing which phase is being requested. A GeometryProxy is also provided, allowing effects to change based on the view’s geometry.

In the following example, the `Text` will have a scale of 1.0 when inactive, and then scale to 1.1 when hovered:

```
Text("Hello, World!")
    .hoverEffect { effect, isActive, proxy in
        effect.scaleEffect(!isActive ? 1.0 : 1.1)
    }
```

Use the animation(_:body:) modifier to specify how visual changes should be animated.

## See Also

### Changing view appearance for hover events

func hoverEffect(HoverEffect) -> some View

Applies a hover effect to this view.

struct HoverEffect

An effect applied when the pointer hovers over a view.

func hoverEffect(some CustomHoverEffect, in: HoverEffectGroup?, isEnabled: Bool) -> some View

Applies a hover effect to this view, optionally adding it to a HoverEffectGroup.

protocol CustomHoverEffect

A type that represents how a view should change when a pointer hovers over a view, or when someone looks at the view.

struct HoverEffectGroup

Describes a grouping of effects that activate together.

func hoverEffectGroup() -> some View

Adds an implicit HoverEffectGroup to all effects defined on descendant views, so that all effects added to subviews activate as a group whenever this view or any descendant views are hovered.

func hoverEffectGroup(HoverEffectGroup?) -> some View

Adds a HoverEffectGroup to all effects defined on descendant views, and activates the group whenever this view or any descendant views are hovered.

func hoverEffectGroup(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior) -> some View

Adds a HoverEffectGroup to all effects defined on descendant views, and activates the group whenever this view or any descendant views are hovered.

protocol HoverEffectContent

A type that describes the effects of a view for a particular hover effect phase.

struct EmptyHoverEffectContent

An empty base effect that you use to build other effects.

func handPointerBehavior(HandPointerBehavior?) -> some View

Sets the behavior of the hand pointer while the user is interacting with the view.

struct HandPointerBehavior

A behavior that can be applied to the hand pointer while the user is interacting with a view.

