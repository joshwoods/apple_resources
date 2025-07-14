

- AppKit
-  NSTextFieldDelegate 

Protocol

# NSTextFieldDelegate

A protocol that a text field delegate can use to control its field editor action menu.

macOS

``` source
protocol NSTextFieldDelegate : NSControlTextEditingDelegate
```

## Topics

### Controlling Editing Behavior

func textField(NSTextField, textView: NSTextView, candidates: [NSTextCheckingResult], forSelectedRange: NSRange) -> [NSTextCheckingResult]

func textField(NSTextField, textView: NSTextView, candidatesForSelectedRange: NSRange) -> [Any]?

func textField(NSTextField, textView: NSTextView, shouldSelectCandidateAt: Int) -> Bool

## Relationships

### Inherits From

- NSControlTextEditingDelegate
- NSObjectProtocol

### Inherited By

- NSComboBoxDelegate
- NSSearchFieldDelegate
- NSTokenFieldDelegate

## See Also

### Text views

class NSTextField

Text the user can select or edit to send an action message to a target when the user presses the Return key.

class NSTextView

A view that draws text and handles user interactions with that text.

protocol NSTextViewDelegate

A set of optional methods that text view delegates can use to manage selection, set text attributes, work with the spell checker, and more.

protocol NSTextDelegate

A set of optional methods implemented by the delegate of an NSText object to edit text and change text formats.

class NSText

The most general programmatic interface for objects that manage text.

