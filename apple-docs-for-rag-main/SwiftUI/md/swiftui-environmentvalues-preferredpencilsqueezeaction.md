

- SwiftUI
- EnvironmentValues
-  preferredPencilSqueezeAction 

Instance Property

# preferredPencilSqueezeAction

The action that the user prefers to perform when squeezing their Apple Pencil, as selected in the Settings app.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+

``` source
var preferredPencilSqueezeAction: PencilPreferredAction { get }
```

## Discussion

You can read this value by creating a property with the Environment property wrapper and using it inside the action closure of the onPencilSqueeze(perform:) view modifier as an indication of what to do when the user squeezes their Apple Pencil:

```
@Environment(\.preferredPencilSqueezeAction) private var preferredAction

var body: some View {
    MyDrawingCanvas()
        .onPencilSqueeze { phase in
            switch (phase, preferredAction) {
                ...
            }
        }
}
```

In macOS, this value cannot be changed by users and is always set to showContextualPalette.

## See Also

### Recognizing Apple Pencil gestures

func onPencilDoubleTap(perform: (PencilDoubleTapGestureValue) -> Void) -> some View

Adds an action to perform after the user double-taps their Apple Pencil.

func onPencilSqueeze(perform: (PencilSqueezeGesturePhase) -> Void) -> some View

Adds an action to perform when the user squeezes their Apple Pencil.

var preferredPencilDoubleTapAction: PencilPreferredAction

The action that the user prefers to perform after double-tapping their Apple Pencil, as selected in the Settings app.

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

