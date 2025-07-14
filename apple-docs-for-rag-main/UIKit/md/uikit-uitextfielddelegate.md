

- UIKit
-  UITextFieldDelegate 

Protocol

# UITextFieldDelegate

A set of optional methods to manage editing and validating text in a text field object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITextFieldDelegate : NSObjectProtocol
```

## Overview

A text field calls the methods of its delegate in response to important changes. You use these methods to validate text that was typed by the user, to respond to specific interactions with the keyboard, and to control the overall editing process. Editing begins shortly before the text field becomes the first responder and displays the keyboard (or its assigned input view). The flow of the editing process is as follows:

1.  Before becoming the first responder, the text field calls its delegate’s textFieldShouldBeginEditing(_:) method. Use that method to allow or prevent the editing of the text field’s contents.

2.  The text field becomes the first responder.

In response, the system displays the keyboard (or the text field’s input view) and posts the keyboardWillShowNotification and keyboardDidShowNotification notifications as needed. If the keyboard or another input view was already visible, the system posts the keyboardWillChangeFrameNotification and keyboardDidChangeFrameNotification notifications instead. 3. The text field calls its delegate’s textFieldDidBeginEditing(_:) method and posts a textDidBeginEditingNotification notification. 4. The text field calls various delegate methods during editing:

- Whenever the current text changes, it calls the textField(_:shouldChangeCharactersIn:replacementString:) method and posts the textDidChangeNotification notification.

- It calls the textFieldShouldClear(_:) method when the user taps the built-in button to clear the text.

- It calls the textFieldShouldReturn(_:) method when the user taps the keyboard’s return button.

5.  Before resigning as first responder, the text field calls its delegate’s textFieldShouldEndEditing(_:) method. Use that method to validate the current text.

6.  The text field resigns as first responder.

In response, the system hides or adjusts the keyboard as needed. When hiding the keyboard, the system posts the keyboardWillHideNotification and keyboardDidHideNotification notifications. 7. The text field calls its delegate’s textFieldDidEndEditing(_:) method and posts a textDidEndEditingNotification notification.

For more information about the features of a text field, see UITextField.

## Topics

### Managing editing

func textFieldShouldBeginEditing(UITextField) -> Bool

Asks the delegate whether to begin editing in the specified text field.

func textFieldDidBeginEditing(UITextField)

Tells the delegate when editing begins in the specified text field.

func textFieldShouldEndEditing(UITextField) -> Bool

Asks the delegate whether to stop editing in the specified text field.

func textFieldDidEndEditing(UITextField, reason: UITextField.DidEndEditingReason)

Tells the delegate when editing stops for the specified text field, and the reason it stopped.

func textFieldDidEndEditing(UITextField)

Tells the delegate when editing stops for the specified text field.

enum DidEndEditingReason

Constants that indicate the reason for ending editing in a text field.

### Editing the text field’s text

func textField(UITextField, shouldChangeCharactersIn: NSRange, replacementString: String) -> Bool

Asks the delegate whether to change the specified text.

func textFieldShouldClear(UITextField) -> Bool

Asks the delegate whether to remove the text field’s current contents.

func textFieldShouldReturn(UITextField) -> Bool

Asks the delegate whether to process the pressing of the Return button for the text field.

### Managing text selection

func textFieldDidChangeSelection(UITextField)

Tells the delegate when the text selection changes in the specified text field.

### Providing a context menu

func textField(UITextField, editMenuForCharactersIn: NSRange, suggestedActions: [UIMenuElement]) -> UIMenu?

Asks the delegate for the menu to display in the text field, based on the text range and actions the system provides.

### Customizing an edit menu

func textField(UITextField, willPresentEditMenuWith: any UIEditMenuInteractionAnimating)

Tells the delegate that the system is about to present an edit menu with an animator.

func textField(UITextField, willDismissEditMenuWith: any UIEditMenuInteractionAnimating)

Tells the delegate that the system is about to dismiss an edit menu with an animator.

### Inserting a Smart Reply suggestion

func textField(UITextField, insertInputSuggestion: UIInputSuggestion)

Tells the delegate when the keyboard delivers an input suggestion.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UISearchTextFieldDelegate

## See Also

### Validating and handling edits

var delegate: (any UITextFieldDelegate)?

The text field’s delegate.

