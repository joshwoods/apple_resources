

- UIKit
- UITextField
-  delegate 

Instance Property

# delegate

The text field’s delegate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UITextFieldDelegate)? { get set }
```

## Discussion

A text field delegate responds to editing-related messages from the text field. You can use the delegate to respond to the text entered by the user and to some special commands, such as when the user taps Return.

Note

If the text field is a UISearchTextField, set its delegate to an object that also conforms to the UISearchTextFieldDelegate protocol.

## See Also

### Validating and handling edits

protocol UITextFieldDelegate

A set of optional methods to manage editing and validating text in a text field object.

