

- SwiftUI
- View
-  glassBackgroundEffect(\_:in:displayMode:) 

Instance Method

# glassBackgroundEffect(\_:in:displayMode:)

Fills the view’s background with a custom glass background effect and a shape that you specify.

visionOS 2.4+

``` source
nonisolated
func glassBackgroundEffect(
    _ effect: S,
    in shape: T,
    displayMode: GlassBackgroundDisplayMode = .always
) -> some View where T : InsettableShape, S : GlassBackgroundEffect
```

## Parameters 

`effect`  

A GlassBackgroundEffect instance that SwiftUI uses to the fill the background shape that you specify.

`shape`  

An InsettableShape instance that SwiftUI draws behind the view.

`displayMode`  

When to display the glass background. The default is GlassBackgroundDisplayMode.always.

## Return Value

A view with a glass background.

