

- UIKit
-  Apple Pencil interactions 

API Collection

# Apple Pencil interactions

Handle user interactions like double tap and squeeze on Apple Pencil.

## Overview

Apple Pencil interactions let a person perform certain actions in your app by double-tapping or squeezing an Apple Pencil. Support Apple Pencil interactions to give people a quick way to perform their preferred action, such as switching between drawing tools, or a custom action that you define in your app.

- To learn more about supporting double-tap and squeeze interactions, read Handling double taps from Apple Pencil and Handling squeezes from Apple Pencil.

- To learn more about handling touches, read Handling input from Apple Pencil.

- To learn more about incorporating hand-drawn content in your app, see Drawing with PencilKit.

Note

Only Apple Pencil Pro supports squeeze interactions. The first-generation Apple Pencil doesn’t support Apple Pencil interactions.

## Topics

### Essentials

Handling double taps from Apple Pencil

Detect and respond to double taps a person makes on Apple Pencil.

Handling squeezes from Apple Pencil

Detect and respond to squeezes a person makes on Apple Pencil Pro.

Handling input from Apple Pencil

Learn how to detect and respond to touches from Apple Pencil.

### Apple Pencil interactions in SwiftUI

nonisolated func onPencilDoubleTap(perform action: @escaping (PencilDoubleTapGestureValue) -> Void) -> some View 

Adds an action to perform after the user double-taps their Apple Pencil.

struct PencilDoubleTapGestureValue

Describes the value of an Apple Pencil double-tap gesture.

nonisolated func onPencilSqueeze(perform action: @escaping (PencilSqueezeGesturePhase) -> Void) -> some View 

Adds an action to perform when the user squeezes their Apple Pencil.

@frozen enum PencilSqueezeGesturePhase

Describes the phase and value of an Apple Pencil squeeze gesture.

struct PencilSqueezeGestureValue

Describes the value of an Apple Pencil squeeze gesture.

struct PencilPreferredAction

An action that the user prefers to perform after double-tapping their Apple Pencil.

struct PencilHoverPose

A value describing the location and distance of an Apple Pencil hovering in the area above a view’s bounds.

### Apple Pencil interactions in UIKit

class UIPencilInteraction

An interaction that tells your app when a person double-taps or squeezes Apple Pencil.

protocol UIPencilInteractionDelegate

The interface an object implements to handle double taps or squeezes a person makes on Apple Pencil.

class Tap

An interaction that represents a double tap on Apple Pencil.

class Squeeze

An interaction that represents a squeeze on Apple Pencil.

enum Phase

Constants that describe the phases of an interaction on Apple Pencil.

class UIPencilHoverPose

An object that describes the hover pose of Apple Pencil during an interaction like double tap or squeeze.

## See Also

### User interactions

Touches, presses, and gestures

Encapsulate your app’s event-handling logic in gesture recognizers so that you can reuse that code throughout your app.

Menus and shortcuts

Simplify interactions with your app using menu systems, contextual menus, Home Screen quick actions, and keyboard shortcuts.

Drag and drop

Bring drag and drop to your app by using interaction APIs with your views.

Pointer interactions

Support pointer interactions in your custom controls and views.

Focus-based navigation

Navigate the interface of your UIKit app using a remote, game controller, or keyboard.

Accessibility for UIKit

Make your UIKit apps accessible to everyone who uses iOS and tvOS.

