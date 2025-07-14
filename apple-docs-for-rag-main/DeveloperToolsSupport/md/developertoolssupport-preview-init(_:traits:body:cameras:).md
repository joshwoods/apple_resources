

- DeveloperToolsSupport
- Preview
-  init(\_:traits:body:cameras:) 

Initializer

# init(\_:traits:body:cameras:)

Creates a preview of a SwiftUI view using the specified traits and custom viewpoints.

visionOS 1.0+

``` source
@MainActor
init(
    _ name: String? = nil,
    traits: PreviewTrait...,
    @ViewBuilder body: @escaping @MainActor () -> any View,
    @PreviewCameraBuilder cameras: () -> [PreviewCamera]
)
```

## Parameters 

`name`  

An optional display name for the preview.

`traits`  

An optional list of PreviewTrait instances that customize the appearance of the preview.

`body`  

A view builder that produces a SwiftUI view to preview.

`cameras`  

One or more preview cameras that indicate the custom, fixed viewpoints that you want to be able to view the preview from.

## Discussion

Preview macros expand into a declaration that calls this initializer. Don’t use this initializer directly. Instead use one of the macros, like Preview(_:traits:body:cameras:).

