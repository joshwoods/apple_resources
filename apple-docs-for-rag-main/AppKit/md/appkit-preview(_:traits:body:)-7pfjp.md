

- AppKit
-  Preview(\_:traits:body:) 

Macro

# Preview(\_:traits:body:)

Preview an NSView.

macOS 14.0+

``` source
@freestanding(declaration)
macro Preview(
    _ name: String? = nil,
    traits: PreviewTrait...,
    @PreviewMacroBodyBuilder body: @escaping @MainActor () -> NSView
)
```

## Parameters 

`name`  

Optional display name for the preview, which will appear in the canvas.

`traits`  

Optional list of traits customizing the appearance of the preview.

`body`  

A closure producing an NSView.

