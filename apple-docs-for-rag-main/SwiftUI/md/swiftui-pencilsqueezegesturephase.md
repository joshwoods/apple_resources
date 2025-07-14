

- SwiftUI
-  PencilSqueezeGesturePhase 

Enumeration

# PencilSqueezeGesturePhase

Describes the phase and value of an Apple Pencil squeeze gesture.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+

``` source
@frozen
enum PencilSqueezeGesturePhase
```

## Overview

When you use the onPencilSqueeze(perform:) view modifier, you can handle the Apple Pencil squeeze gesture’s phase in the `action` closure.

## Topics

### Enumeration Cases

case active(PencilSqueezeGestureValue)

The user started squeezing their Apple Pencil.

case ended(PencilSqueezeGestureValue)

The user successfully completed a squeeze gesture.

case failed

The user started squeezing their Apple Pencil but failed to successfully complete the gesture.

## Relationships

### Conforms To

- Equatable

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

struct PencilHoverPose

A value describing the location and distance of an Apple Pencil hovering in the area above a view’s bounds.

