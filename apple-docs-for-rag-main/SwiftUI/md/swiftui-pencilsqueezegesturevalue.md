

- SwiftUI
-  PencilSqueezeGestureValue 

Structure

# PencilSqueezeGestureValue

Describes the value of an Apple Pencil squeeze gesture.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+

``` source
struct PencilSqueezeGestureValue
```

## Topics

### Instance Properties

let hoverPose: PencilHoverPose?

The location and distance of an Apple Pencil hovering in the area above the view’s bounds when the squeeze gesture occurred.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Recognizing Apple Pencil gestures

func onPencilDoubleTap(perform: (PencilDoubleTapGestureValue) -> Void) -> some View

Adds an action to perform after the user double-taps their Apple Pencil.

func onPencilSqueeze(perform: (PencilSqueezeGesturePhase) -> Void) -> some View

Adds an action to perform when the user squeezes their Apple Pencil.

var preferredPencilDoubleTapAction: PencilPreferredAction

The action that the user prefers to perform after double-tapping their Apple Pencil, as selected in the Settings app.

var preferredPencilSqueezeAction: PencilPreferredAction

The action that the user prefers to perform when squeezing their Apple Pencil, as selected in the Settings app.

struct PencilPreferredAction

An action that the user prefers to perform after double-tapping their Apple Pencil.

struct PencilDoubleTapGestureValue

Describes the value of an Apple Pencil double-tap gesture.

enum PencilSqueezeGesturePhase

Describes the phase and value of an Apple Pencil squeeze gesture.

struct PencilHoverPose

A value describing the location and distance of an Apple Pencil hovering in the area above a view’s bounds.

