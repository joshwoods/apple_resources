

- UIKit
- UITextView
-  inputView 

Instance Property

# inputView

The custom input view to display when the text view becomes the first responder.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var inputView: UIView? { get set }
```

## Discussion

If the value in this property is `nil`, the text view displays the standard system keyboard when it becomes first responder. Assigning a custom view to this property causes that view to be presented instead.

The default value of this property is `nil`.

## See Also

### Replacing the system input views

var inputAccessoryView: UIView?

The custom accessory view to display when the text view becomes the first responder.

