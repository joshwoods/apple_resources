

- DeveloperToolsSupport
- Preview
-  init(\_:traits:body:) 

Initializer

# init(\_:traits:body:)

Creates a preview of a SwiftUI view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor
init(
    _ name: String? = nil,
    traits: PreviewTrait...,
    body: @escaping @MainActor () -> any View
)
```

## Parameters 

`name`  

An optional display name for the preview.

`traits`  

An optional list of PreviewTrait instances that customize the appearance of the preview.

`body`  

A view builder that produces a SwiftUI view to preview.

## Discussion

Preview macros expand into a declaration that calls this initializer. Don’t use this initializer directly. Instead use one of the macros, like Preview(_:body:).

