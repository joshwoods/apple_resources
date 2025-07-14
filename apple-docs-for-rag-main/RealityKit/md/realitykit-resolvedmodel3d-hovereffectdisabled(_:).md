

- RealityKit
- ResolvedModel3D
-  hoverEffectDisabled(\_:) 

Instance Method

# hoverEffectDisabled(\_:)

Adds a condition that controls whether this view can display hover effects.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
func hoverEffectDisabled(_ disabled: Bool = true) -> some View
```

## Parameters 

`disabled`  

A Boolean value that determines whether this view can display hover effects.

## Return Value

A view that controls whether hover effects can be displayed in this view.

## Discussion

The higher views in a view hierarchy can override the value you set on this view. In the following example, the button does not display a hover effect because the outer `hoverEffectDisabled(_:)` modifier overrides the inner one:

```
HStack {
    Button("Press") {}
        .hoverEffectDisabled(false)
}
.hoverEffectDisabled(true)
```

