

- SwiftUI
-  PencilHoverPose 

Structure

# PencilHoverPose

A value describing the location and distance of an Apple Pencil hovering in the area above a view’s bounds.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+

``` source
struct PencilHoverPose
```

## Topics

### Getting the hover characteristics

let anchor: UnitPoint

The location of an Apple Pencil hovering in the area above the view’s bounds, expressed as a normalized anchor point relative to that view.

let location: CGPoint

The location of an Apple Pencil hovering in the area above the view’s bounds, expressed as a point in that view’s coordinate space.

let zDistance: CGFloat

The normalized distance between the screen and a hovering Apple Pencil.

### Instance Properties

let altitude: Angle

A value that represents the altitude angle of the hovering Apple Pencil.

let azimuth: Angle

A value that represents the azimuth angle of a hovering Apple Pencil.

let roll: Angle

A value that represents the barrel roll angle of the hovering Apple Pencil.

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

struct PencilSqueezeGestureValue

Describes the value of an Apple Pencil squeeze gesture.

enum PencilSqueezeGesturePhase

Describes the phase and value of an Apple Pencil squeeze gesture.

