

- DeveloperToolsSupport
- Preview
-  init(\_:windowStyle:traits:body:cameras:) 

Initializer

# init(\_:windowStyle:traits:body:cameras:)

Creates a preview of a SwiftUI view in a window with custom viewpoints.

visionOS 1.0+

``` source
@MainActor
init(
    _ name: String? = nil,
    windowStyle: some WindowStyle,
    traits: PreviewTrait...,
    @ViewBuilder body: @escaping @MainActor () -> any View,
    @PreviewCameraBuilder cameras: () -> [PreviewCamera] = { return [] }
)
```

## Parameters 

`name`  

An optional display name for the preview.

`windowStyle`  

The window style to use for the preview.

`traits`  

An optional list of PreviewTrait instances that customize the appearance of the preview.

`body`  

A view builder that produces a SwiftUI view to preview.

`cameras`  

One or more preview cameras that indicate the custom, fixed viewpoints that you want to be able to view the preview from.

## Discussion

Preview macros expand into a declaration that calls this initializer. Don’t use this initializer directly. Instead use one of the macros, like Preview(_:windowStyle:traits:body:cameras:).

