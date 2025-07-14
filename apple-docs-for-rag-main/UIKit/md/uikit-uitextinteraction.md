

- UIKit
-  UITextInteraction 

Class

# UITextInteraction

An interaction that provides text selection gestures and UI to custom text views.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UITextInteraction
```

## Mentioned in 

Adopting system selection UI in custom text views

## Overview

Use UITextInteraction to provide your custom text views the same text selection gestures and UI available in native text views like UITextView and UITextField. When creating a text interaction, choose a mode that matches the state of the text, UITextInteractionMode.editable or UITextInteractionMode.nonEditable. Then set the textInput property to an object that conforms to UITextInput, and add the interaction to a view.

```
// Create a selection interaction for non-editable content.
let selectionInteraction = UITextInteraction(for: .nonEditable)

// Assign `textInput` to your view that implements the `UITextInput` protocol
// to get more control over the selection behavior and the text input system.
selectionInteraction.textInput = customTextView

// Add the interaction to the view.
customTextView.addInteraction(selectionInteraction)
```

If your custom text view supports editable and non-editable text, create two interactions — one for each mode — and add the interaction that matches the state of text to the view while removing the other interaction.

```
override func becomeFirstResponder() -> Bool {
    let isFirstResponder = self.isFirstResponder
    let result = super.becomeFirstResponder()

    if isFirstResponder == false && self.isFirstResponder == true {
        customTextView.removeInteraction(nonEditableTextInteraction)
        customTextView.addInteraction(editableTextInteraction)
    }

    return result
}

override func resignFirstResponder() -> Bool {
    let isFirstResponder = self.isFirstResponder
    let result = super.resignFirstResponder()

    if isFirstResponder == true && self.isFirstResponder == false {
        customTextView.removeInteraction(editableTextInteraction)
        customTextView.addInteraction(nonEditableTextInteraction)
    }

    return result
}
```

If your app provides other gestures in the same view hierarchy, you can use the require(toFail:) method to set up failure requirements between your app’s gestures and the text interaction gestures listed in the gesturesForFailureRequirements property.

## Topics

### Creating text interactions

convenience init(for: UITextInteractionMode)

Creates a text interaction with the specified mode.

### Handling text input and interaction events

var textInput: (any UIResponder &amp; UITextInput)?

The object that interacts with the text input system.

var delegate: (any UITextInteractionDelegate)?

The object that receives events from the text interaction.

protocol UITextInteractionDelegate

An interface that an object implements to receive information about text interaction events.

### Getting interaction information

var gesturesForFailureRequirements: [UIGestureRecognizer]

The list of gestures that the text interaction adds to the view hierarchy.

var textInteractionMode: UITextInteractionMode

The mode of the text interaction.

enum UITextInteractionMode

Modes that determine the selection behaviors that a text interaction provides.

## Relationships

### Inherits From

- NSObject

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

### Text interactions

protocol UITextInteractionDelegate

An interface that an object implements to receive information about text interaction events.

enum UITextInteractionMode

Modes that determine the selection behaviors that a text interaction provides.

