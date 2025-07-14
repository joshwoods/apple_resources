

- AppKit
-  Gestures 

API Collection

# Gestures

Encapsulate your app’s event-handling logic in gesture recognizers so that you can reuse that code throughout your app.

## Topics

### Standard Gestures

class NSClickGestureRecognizer

A discrete gesture recognizer that tracks a specified number of mouse clicks.

class NSPressGestureRecognizer

A discrete gesture recognizer that tracks whether the user holds down a mouse button for a minimum amount of time before releasing it.

class NSPanGestureRecognizer

A continuous gesture recognizer for panning gestures.

class NSRotationGestureRecognizer

A continuous gesture recognizer that tracks two trackpad touches moving opposite each other in a circular motion.

class NSMagnificationGestureRecognizer

A continuous gesture recognizer that tracks a pinch gesture that magnifies content.

### Custom Gestures

class NSGestureRecognizer

An object that monitors events and calls its action method when a predefined sequence of events occur.

protocol NSGestureRecognizerDelegate

A set of methods for fine-tuning a gesture recognizer’s behavior.

## See Also

### User Interactions

Mouse, Keyboard, and Trackpad

Handle events related to mouse, keyboard, and trackpad input.

Menus, Cursors, and the Dock

Implement menus and cursors to facilitate interactions with your app, and use your app’s Dock tile to convey updated information.

Touch Bar

Display interactive content and controls in the Touch Bar.

Drag and Drop

Support the direct manipulation of your app’s content using drag and drop.

Accessibility for AppKit

Make your AppKit apps accessible to everyone who uses macOS.

