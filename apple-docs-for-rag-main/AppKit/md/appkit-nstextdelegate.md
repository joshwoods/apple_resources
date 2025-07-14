

- AppKit
-  NSTextDelegate 

Protocol

# NSTextDelegate

A set of optional methods implemented by the delegate of an NSText object to edit text and change text formats.

macOS

``` source
protocol NSTextDelegate : NSObjectProtocol
```

## Topics

### Changing text formatting

func textDidChange(Notification)

Informs the delegate that the text object has changed its characters or formatting attributes.

### Editing text

func textShouldBeginEditing(NSText) -> Bool

Invoked when a text object begins to change its text, this method requests permission for `aTextObject` to begin editing.

func textDidBeginEditing(Notification)

Informs the delegate that the text object has begun editing (that the user has begun changing it).

func textShouldEndEditing(NSText) -> Bool

Invoked from a text object’s implementation of resignFirstResponder(), this method requests permission for `aTextObject` to end editing.

func textDidEndEditing(Notification)

Informs the delegate that the text object has finished editing (that it has resigned first responder status).

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSTextViewDelegate

### Conforming Types

- NSOutlineView
- NSTableView

## See Also

### Text views

class NSTextField

Text the user can select or edit to send an action message to a target when the user presses the Return key.

protocol NSTextFieldDelegate

A protocol that a text field delegate can use to control its field editor action menu.

class NSTextView

A view that draws text and handles user interactions with that text.

protocol NSTextViewDelegate

A set of optional methods that text view delegates can use to manage selection, set text attributes, work with the spell checker, and more.

class NSText

The most general programmatic interface for objects that manage text.

