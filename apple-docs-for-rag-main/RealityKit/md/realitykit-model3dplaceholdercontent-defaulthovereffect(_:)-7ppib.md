

- RealityKit
- Model3DPlaceholderContent
-  defaultHoverEffect(\_:) 

Instance Method

# defaultHoverEffect(\_:)

Sets the default hover effect to use for views within this view.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
func defaultHoverEffect(_ effect: HoverEffect?) -> some View
```

## Parameters 

`effect`  

The default hover effect to use for views within this view.

## Return Value

A view that uses this effect as the default hover effect.

## Discussion

Use this modifier to set a specific hover effect for all views with the `View/hoverEffect(_:)` modifier applied within a view. The default effect is typically used when no `HoverEffect` was provided or if `HoverEffect/automatic` is specified.

For example, this view uses `HoverEffect/highlight` for both the red and green Color views:

```
HStack {
    Color.red.hoverEffect()
    Color.green.hoverEffect()
}
.defaultHoverEffect(.highlight)
```

This also works for customizing the default hover effect in views like `Button`s when using a SwiftUI-defined style like `ButtonStyle/bordered`, which can provide a hover effect by default. For example, this view replaces the hover effect for a `Button` with `HoverEffect/highlight`:

```
Button("Next") {}
    // perform action
}
.buttonStyle(.bordered)
.defaultHoverEffect(.highlight)
```

Use a `nil` effect to indicate that the default hover effect should not be modified.

