

- UIKit
-  UITextDroppable 

Protocol

# UITextDroppable

The interface that determines if a text view is a drop destination.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITextDroppable : UITextInput, UITextPasteConfigurationSupporting
```

## Topics

### Checking the text drop activity status

var isTextDropActive: Bool

A Boolean value that indicates whether the text view has at least one active drop session.

**Required**

### Managing the text drop interaction

var textDropInteraction: UIDropInteraction?

The drop interaction object added by UIKit to the text view.

**Required**

### Setting the text drop delegate

var textDropDelegate: (any UITextDropDelegate)?

The text drop delegate for interacting with a drop activity in the text view.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UIKeyInput
- UIPasteConfigurationSupporting
- UITextInput
- UITextInputTraits
- UITextPasteConfigurationSupporting

### Conforming Types

- UISearchTextField
- UITextField
- UITextView

## See Also

### Text view additions

protocol UITextDragDelegate

The interface for customizing the behavior of a drag activity for a text view.

protocol UITextDropDelegate

The interface for configuring a text view’s drop behavior.

protocol UITextDraggable

The interface that determines if a text view is a drag source.

struct UITextDragOptions

A set of options that determine the behavior of a draggable text view.

enum UITextDropEditability

The text-drop editability styles for noneditable text views.

