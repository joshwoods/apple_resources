

- Assignables
- AssignableDocumentView
-  overlay(\_:alignment:) 

Instance Method

# overlay(\_:alignment:)

Layers a secondary view in front of this view.

AssignablesSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func overlay(
    _ overlay: Overlay,
    alignment: Alignment = .center
) -> some View where Overlay : View
```

## Parameters 

`overlay`  

The view to layer in front of this view.

`alignment`  

The alignment for `overlay` in relation to this view.

## Return Value

A view that layers `overlay` in front of the view.

## Discussion

When you apply an overlay to a view, the original view continues to provide the layout characteristics for the resulting view. In the following example, the heart image is shown overlaid in front of, and aligned to the bottom of the folder image.

```
Image(systemName: "folder")
    .font(.system(size: 55, weight: .thin))
    .overlay(Text("❤️"), alignment: .bottom)
```

