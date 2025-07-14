

- SwiftUI
-  Preview(\_:immersionStyle:traits:body:cameras:) 

Macro

# Preview(\_:immersionStyle:traits:body:cameras:)

Creates a preview of a SwiftUI view in an immersive space with custom viewpoints.

visionOS 1.0+

``` source
@freestanding(declaration)
macro Preview(
    _ name: String? = nil,
    immersionStyle: Style,
    traits: PreviewTrait...,
    @ViewBuilder body: @escaping @MainActor () -> any View,
    @PreviewCameraBuilder cameras: () -> [PreviewCamera]
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

`cameras`  

One or more preview cameras that indicate the custom, fixed viewpoints that you want to be able to view the preview from. The first of these replaces the front viewpoint as the default.

## Overview

This preview macro behaves like Preview(_:immersionStyle:traits:body:) combined with Preview(_:traits:body:cameras:): it enables you to define an immersive space scene context for the view, and also to define custom, fixed viewpoints for the preview:

```
#Preview("Mixed immersive space", immersionStyle: .mixed) {
   ContentView()
} cameras: {
   PreviewCamera(from: .front)
   PreviewCamera(from: .top, zoom: 2)
   PreviewCamera(from: .leading, zoom: 0.5, name: "close up")
}
```

See those other preview macros for more information about using scenes and cameras in your preview. If you want to preview in a window rather than an immersive space, use Preview(_:windowStyle:traits:body:cameras:).

## See Also

### Creating a preview in the context of a scene

macro Preview&lt;Style>(String?, immersionStyle: Style, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View)

Creates a preview of a SwiftUI view in an immersive space.

macro Preview&lt;Style>(String?, windowStyle: Style, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View)

Creates a preview of a SwiftUI view in a window.

macro Preview&lt;Style>(String?, windowStyle: Style, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View, cameras: () -> [PreviewCamera])

Creates a preview of a SwiftUI view in a window with custom viewpoints.

