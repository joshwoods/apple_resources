

- SwiftUI
-  Preview(\_:immersionStyle:traits:body:) 

Macro

# Preview(\_:immersionStyle:traits:body:)

Creates a preview of a SwiftUI view in an immersive space.

visionOS 1.0+

``` source
@freestanding(declaration)
macro Preview(
    _ name: String? = nil,
    immersionStyle: Style,
    traits: PreviewTrait...,
    @ViewBuilder body: @escaping @MainActor () -> any View
) where Style : ImmersionStyle
```

## Parameters 

`name`  

An optional display name for the preview. If you don’t specify a name, the canvas labels the preview using the line number where the preview appears in source.

`immersionStyle`  

The ImmersionStyle to use for the preview. Use this input to display the view as if it appears in an immersive space that has the specified style.

`traits`  

An optional list of PreviewTrait instances that customize the appearance of the preview.

`body`  

A ViewBuilder that produces a SwiftUI view to preview. You typically specify one of your app’s custom views and optionally any inputs, model data, modifiers, and enclosing views that the custom view needs for normal operation.

## Overview

This preview macro behaves like Preview(_:traits:_:body:), except that it also enables you to define a scene context for the view. Specifically, it places the view in an immersive space with the specified immersion style, like the mixed style:

```
#Preview("Mixed immersive space", immersionStyle: .mixed) {
   ContentView()
}
```

Use this preview macro when the view needs scene context to behave as it would during normal operation of your app.

Other preview macros provide different customization options. For example, if you want to see how the view appears in a window rather than an immersive space, you can use Preview(_:windowStyle:traits:body:). If you want to add custom, fixed viewpoints to an immersive space preview, use Preview(_:immersionStyle:traits:body:cameras:).

## See Also

### Creating a preview in the context of a scene

macro Preview&lt;Style>(String?, immersionStyle: Style, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View, cameras: () -> [PreviewCamera])

Creates a preview of a SwiftUI view in an immersive space with custom viewpoints.

macro Preview&lt;Style>(String?, windowStyle: Style, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View)

Creates a preview of a SwiftUI view in a window.

macro Preview&lt;Style>(String?, windowStyle: Style, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View, cameras: () -> [PreviewCamera])

Creates a preview of a SwiftUI view in a window with custom viewpoints.

