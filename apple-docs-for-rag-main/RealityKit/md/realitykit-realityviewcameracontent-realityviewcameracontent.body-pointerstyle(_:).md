

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  pointerStyle(\_:) 

Instance Method

# pointerStyle(\_:)

Sets the pointer style to display when the pointer is over the view.

RealityKitSwiftUImacOS 15.0+visionOS 2.0+

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

Refer to `PointerStyle` for a list of available pointer styles.

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

