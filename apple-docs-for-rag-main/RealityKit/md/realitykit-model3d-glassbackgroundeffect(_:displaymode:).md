

- RealityKit
- Model3D
-  glassBackgroundEffect(\_:displayMode:) 

Instance Method

# glassBackgroundEffect(\_:displayMode:)

Fills the view’s background with a custom glass background effect and container-relative rounded rectangle shape.

RealityKitSwiftUIvisionOS 2.4+

``` source
nonisolated
func glassBackgroundEffect(
    _ effect: S,
    displayMode: GlassBackgroundDisplayMode = .always
) -> some View where S : GlassBackgroundEffect
```

## Parameters 

`effect`  

A `GlassBackgroundEffect` instance that SwiftUI uses to draw a background of the modified view.

`displayMode`  

When to display the glass background. The default is `GlassBackgroundDisplayMode/always`.

## Return Value

A view with a glass background.

## Discussion

Use this modifier to add a glass material that may include thickness, specularity, glass blur, shadows, and other effects. Because of its physical depth, the background influences z-axis layout. For different effect, the bakcground may influences x-axis and y-axis layout.

To ensure that the effect renders properly when you add it to a collection of views in a `ZStack`, add the modifier to the stack rather to one of the views in the stack. This includes when you create an implicit stack with view modifiers like `View/overlay(alignment:content:)` or `View/background(alignment:content:)`. In those cases, you might need to create an explicit `ZStack` inside the `content` closure to have a place to add the background modifier.

Non closed shapes will be rendered as their convex hull.

