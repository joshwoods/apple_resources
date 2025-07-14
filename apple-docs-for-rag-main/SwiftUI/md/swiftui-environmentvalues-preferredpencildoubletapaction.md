

- SwiftUI
- EnvironmentValues
-  preferredPencilDoubleTapAction 

Instance Property

# preferredPencilDoubleTapAction

The action that the user prefers to perform after double-tapping their Apple Pencil, as selected in the Settings app.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+

``` source
var preferredPencilDoubleTapAction: PencilPreferredAction { get }
```

## Discussion

You can read this value by creating a property with the Environment property wrapper and using it inside the action closure of the onPencilDoubleTap(perform:) view modifier as an indication of what to do after the user double-taps their Apple Pencil:

```
@Environment(\.preferredPencilDoubleTapAction) private var preferredAction

var body: some View {
    MyDrawingCanvas()
        .onPencilDoubleTap { value in
            switch preferredAction {
                ...
            }
        }
}
```

In macOS, this value cannot be changed by users and is always set to switchEraser.

## See Also

### Recognizing Apple Pencil gestures

func onPencilDoubleTap(perform: (PencilDoubleTapGestureValue) -> Void) -> some View

Adds an action to perform after the user double-taps their Apple Pencil.

func onPencilSqueeze(perform: (PencilSqueezeGesturePhase) -> Void) -> some View

Adds an action to perform when the user squeezes their Apple Pencil.

var preferredPencilSqueezeAction: PencilPreferredAction

The action that the user prefers to perform when squeezing their Apple Pencil, as selected in the Settings app.

struct PencilPreferredAction

An action that the user prefers to perform after double-tapping their Apple Pencil.

struct PencilDoubleTapGestureValue

Describes the value of an Apple Pencil double-tap gesture.

struct PencilSqueezeGestureValue

Describes the value of an Apple Pencil squeeze gesture.

enum PencilSqueezeGesturePhase

Describes the phase and value of an Apple Pencil squeeze gesture.

struct PencilHoverPose

A value describing the location and distance of an Apple Pencil hovering in the area above a view’s bounds.

