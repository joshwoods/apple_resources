

- UIKit
-  UISelectionFeedbackGenerator 

Class

# UISelectionFeedbackGenerator

A concrete feedback generator subclass that creates haptics to indicate a change in selection.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
class UISelectionFeedbackGenerator
```

## Overview

Use selection feedback to communicate movement through a series of discrete values. For example, you might trigger selection feedback to indicate that a UI element’s values are changing.

The following code example shows how to play selection feedback in response to a long-press gesture.

```
var feedback = UISelectionFeedbackGenerator()

override func viewDidLoad() {
    super.viewDidLoad()

    // Create a selection feedback object and associate it with the view.
    feedback = UISelectionFeedbackGenerator(view: view)

    // Add a custom long-press gesture to the view.
    let longPressGesture = UILongPressGestureRecognizer(target: self, action: #selector(longPress(_:)))
    longPressGesture.numberOfTouchesRequired = 2
    view.addGestureRecognizer(longPressGesture)
}

@objc
private func longPress(_ sender: UILongPressGestureRecognizer) {
    if sender.state == .began {
        // Play selection feedback to indicate a selection change.
        feedback.selectionChanged(at: sender.location(in: view))

        // Update the UI in response to a selection change.
        // ...
    }
}
```

For more information, read Playing haptic feedback in your app.

## Topics

### Reporting selection changes

func selectionChanged()

Triggers selection feedback.

func selectionChanged(at: CGPoint)

Triggers selection feedback at the specified location.

## Relationships

### Inherits From

- UIFeedbackGenerator

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIInteraction

## See Also

### Haptic feedback

Playing haptic feedback in your app

Provide tactile feedback when people perform certain actions in your app.

class UIFeedbackGenerator

The abstract superclass for all feedback generators.

class UIImpactFeedbackGenerator

A concrete feedback generator subclass that creates haptics to simulate physical impacts.

class UINotificationFeedbackGenerator

A concrete feedback generator subclass that creates haptics to communicate successes, failures, and warnings.

class UICanvasFeedbackGenerator

A concrete feedback generator subclass that creates haptics to indicate events on a drawing canvas.

