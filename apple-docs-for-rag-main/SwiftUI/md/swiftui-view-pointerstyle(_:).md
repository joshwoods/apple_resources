

- SwiftUI
- View
-  pointerStyle(\_:) 

Instance Method

# pointerStyle(\_:)

Sets the pointer style to display when the pointer is over the view.

macOS 15.0+visionOS 2.0+

``` source
nonisolated
func pointerStyle(_ style: PointerStyle?) -> some View
```

## Parameters 

`style`  

The pointer style to use.

## Return Value

A view that changes the style of the pointer when hovered.

## Discussion

Refer to PointerStyle for a list of available pointer styles.

For guidance on choosing an appropriate pointer style, refer to Pointing devices in the Human Interface Guidelines.

In this example, the pointer style indicates rectangular selection is possible while the Option modifier key is pressed:

```
enum ToolMode {
    // ...
    case selection
}

struct ImageEditorView: View {
    @State private var toolMode?

    var body: some View {
        ImageCanvasView()
            .pointerStyle(
                toolMode == .selection ? .rectSelection : nil)
            .onModifierKeysChanged { _, modifierKeys in
                if modifierKeys.contains(.option) {
                    toolMode = .selection
                } else {
                    toolMode = nil
                }
            }
    }
}
```

## See Also

### Modifying pointer appearance

struct PointerStyle

A style describing the appearance of the pointer (also called a cursor) when it’s hovered over a view.

func pointerVisibility(Visibility) -> some View

Sets the visibility of the pointer when it’s over the view.

enum HorizontalDirection

A direction on the horizontal axis.

enum VerticalDirection

A direction on the horizontal axis.

enum FrameResizePosition

The position along the perimeter of a rectangular frame (its edges and corners) from which it’s resized.

enum FrameResizeDirection

The direction in which a rectangular frame can be resized.

