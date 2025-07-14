

- UIKit
-  UITextDraggable 

Protocol

# UITextDraggable

The interface that determines if a text view is a drag source.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITextDraggable : UITextInput
```

## Topics

### Checking the text drag activity status

var isTextDragActive: Bool

A Boolean value indicating whether at least one drag session for the text view is active.

**Required**

### Managing the text drag interaction

var textDragInteraction: UIDragInteraction?

The drag interaction object added by UIKit to the text view.

**Required**

### Setting the text drag delegate

var textDragDelegate: (any UITextDragDelegate)?

A text drag delegate object for customizing the drag source behavior of a text view.

**Required**

### Setting the text drag options

var textDragOptions: UITextDragOptions

The options for the text drag operation.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UIKeyInput
- UITextInput
- UITextInputTraits

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

struct UITextDragOptions

A set of options that determine the behavior of a draggable text view.

protocol UITextDroppable

The interface that determines if a text view is a drop destination.

enum UITextDropEditability

The text-drop editability styles for noneditable text views.

