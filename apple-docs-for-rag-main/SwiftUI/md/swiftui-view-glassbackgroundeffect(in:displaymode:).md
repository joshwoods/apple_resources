

- SwiftUI
- View
-  glassBackgroundEffect(in:displayMode:) 

Instance Method

# glassBackgroundEffect(in:displayMode:)

Fills the view’s background with an automatic glass background effect and a shape that you specify.

visionOS 1.0+

``` source
nonisolated
func glassBackgroundEffect(
    in shape: S,
    displayMode: GlassBackgroundDisplayMode = .always
) -> some View where S : InsettableShape
```

## Parameters 

`shape`  

An InsettableShape instance that SwiftUI draws behind the view.

`displayMode`  

When to display the glass background. The default is GlassBackgroundDisplayMode.always.

## Return Value

A view with a glass background.

## Discussion

Use this modifier to add a 3D glass background material that includes thickness, specularity, glass blur, shadows, and other effects. Because of its physical depth, the glass background influences z-axis layout.

To ensure that the effect renders properly when you add it to a collection of views in a ZStack, add the modifier to the stack rather to one of the views in the stack. This includes when you create an implicit stack with view modifiers like overlay(alignment:content:) or background(alignment:content:). In those cases, you might need to create an explicit ZStack inside the `content` closure to have a place to add the glass background modifier.

Non closed shapes will be rendered as their convex hull.

## See Also

### Adding a glass background

func glassBackgroundEffect(displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with an automatic glass background effect and container-relative rounded rectangle shape.

enum GlassBackgroundDisplayMode

The display mode of a glass background.

