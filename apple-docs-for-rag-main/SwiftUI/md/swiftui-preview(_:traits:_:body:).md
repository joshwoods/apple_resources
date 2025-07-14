

- SwiftUI
-  Preview(\_:traits:\_:body:) 

Macro

# Preview(\_:traits:\_:body:)

Creates a preview of a SwiftUI view using the specified traits.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@freestanding(declaration)
macro Preview(
    _ name: String? = nil,
    traits: PreviewTrait,
    _ additionalTraits: PreviewTrait...,
    @ViewBuilder body: @escaping @MainActor () -> any View
)
```

## Parameters 

`name`  

An optional display name for the preview. If you don’t specify a name, the canvas labels the preview using the line number where the preview appears in source.

`traits`  

A PreviewTrait instance that customizes the appearance of the preview.

`additionalTraits`  

Optional additional traits that further customize the preview.

`body`  

A ViewBuilder that produces a SwiftUI view to preview. You typically specify one of your app’s custom views and optionally any inputs, model data, modifiers, and enclosing views that the custom view needs for normal operation.

## Overview

This macro behaves like Preview(_:body:) except that it also enables you to customize the appearance of the preview by adding one or more traits, which are instances of PreviewTrait. For example, you can display a preview at a fixed size using the fixedLayout(width:height:) trait:

```
#Preview(
    "Content",
    traits: .fixedLayout(width: 100, height: 100)
) {
    ContentView()
}
```

The macro ignores traits that don’t apply to the current context. For example, the portrait trait has no impact on a visionOS preview.

Other preview macros provide different customization options. For example, if you want to specify a custom viewpoint for the preview, use Preview(_:traits:body:cameras:).

## See Also

### Creating a preview

macro Preview(String?, body: () -> any View)

Creates a preview of a SwiftUI view.

macro Preview(String?, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View, cameras: () -> [PreviewCamera])

Creates a preview of a SwiftUI view using the specified traits and custom viewpoints.

