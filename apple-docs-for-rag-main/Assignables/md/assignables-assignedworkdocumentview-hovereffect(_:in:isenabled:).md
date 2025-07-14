

- Assignables
- AssignedWorkDocumentView
-  hoverEffect(\_:in:isEnabled:) 

Instance Method

# hoverEffect(\_:in:isEnabled:)

Applies a hover effect to this view, optionally adding it to a `HoverEffectGroup`.

AssignablesSwiftUIvisionOS 2.0+

``` source
nonisolated
func hoverEffect(
    _ effect: some CustomHoverEffect,
    in group: HoverEffectGroup?,
    isEnabled: Bool = true
) -> some View
```

## Parameters 

`effect`  

The effect to apply to this view.

`group`  

An optional `HoverEffectGroup` the effect should belong to.

`isEnabled`  

Whether this effect is enabled or not.

## Return Value

A new view that applies the hover effect to `self` whenever the view is hovered, or the `HoverEffectGroup` is activated.

