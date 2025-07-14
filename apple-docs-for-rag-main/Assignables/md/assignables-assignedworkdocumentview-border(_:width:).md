

- Assignables
- AssignedWorkDocumentView
-  border(\_:width:) 

Instance Method

# border(\_:width:)

Adds a border to this view with the specified style and width.

AssignablesSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func border(
    _ content: S,
    width: CGFloat = 1
) -> some View where S : ShapeStyle
```

## Parameters 

`content`  

A value that conforms to the `ShapeStyle` protocol, like a `Color` or `HierarchicalShapeStyle`, that SwiftUI uses to fill the border.

`width`  

The thickness of the border. The default is 1 pixel.

## Return Value

A view that adds a border with the specified style and width to this view.

## Discussion

Use this modifier to draw a border of a specified width around the view’s frame. By default, the border appears inside the bounds of this view. For example, you can add a four-point wide border covers the text:

```
Text("Purple border inside the view bounds.")
    .border(Color.purple, width: 4)
```

To place a border around the outside of this view, apply padding of the same width before adding the border:

```
Text("Purple border outside the view bounds.")
    .padding(4)
    .border(Color.purple, width: 4)
```

