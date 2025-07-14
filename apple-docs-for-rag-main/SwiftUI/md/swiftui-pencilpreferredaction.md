

- SwiftUI
-  PencilPreferredAction 

Structure

# PencilPreferredAction

An action that the user prefers to perform after double-tapping their Apple Pencil.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+

``` source
struct PencilPreferredAction
```

## Topics

### Getting the preffered actions

static let ignore: PencilPreferredAction

An action that does nothing.

static let showColorPalette: PencilPreferredAction

An action that toggles the display of the color palette.

static let showInkAttributes: PencilPreferredAction

An action that toggles the display of the current tool’s ink attributes.

static let switchEraser: PencilPreferredAction

An action that switches between the current tool and the eraser.

static let switchPrevious: PencilPreferredAction

An action that switches between the current tool and the last used tool.

### Type Properties

static let runSystemShortcut: PencilPreferredAction

An action that runs a system shortcut.

static let showContextualPalette: PencilPreferredAction

An action that toggles the display of the contextual palette, or the undo/redo panel if contextual palette is not available.

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

struct PencilDoubleTapGestureValue

Describes the value of an Apple Pencil double-tap gesture.

struct PencilSqueezeGestureValue

Describes the value of an Apple Pencil squeeze gesture.

enum PencilSqueezeGesturePhase

Describes the phase and value of an Apple Pencil squeeze gesture.

struct PencilHoverPose

A value describing the location and distance of an Apple Pencil hovering in the area above a view’s bounds.

