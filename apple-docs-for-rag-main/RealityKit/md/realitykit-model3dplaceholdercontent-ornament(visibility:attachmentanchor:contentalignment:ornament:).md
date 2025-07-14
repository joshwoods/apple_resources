

- RealityKit
- Model3DPlaceholderContent
-  ornament(visibility:attachmentAnchor:contentAlignment:ornament:) 

Instance Method

# ornament(visibility:attachmentAnchor:contentAlignment:ornament:)

Presents an ornament.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
func ornament(
    visibility: Visibility = .automatic,
    attachmentAnchor: OrnamentAttachmentAnchor,
    contentAlignment: Alignment = .center,
    @ViewBuilder ornament: () -> Content
) -> some View where Content : View
```

## Parameters 

`visibility`  

The visibility of the ornament.

`attachmentAnchor`  

The positioning anchor that defines the attachment point of the ornament.

`contentAlignment`  

The alignment of the ornament with its attachment anchor.

`content`  

The content of the ornament.

## Discussion

Use this method to show an ornament at the specified position. The example below displays an ornament below the window:

```
Text("A view with an ornament")
    .ornament(attachmentAnchor: .scene(.bottom)) {
        OrnamentContent()
    }
```

