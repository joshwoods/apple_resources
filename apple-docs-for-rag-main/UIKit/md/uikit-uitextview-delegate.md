

- UIKit
- UITextView
-  delegate 

Instance Property

# delegate

The text view’s delegate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UITextViewDelegate)? { get set }
```

## Discussion

A text view delegate responds to editing-related messages from the text view. You can use the delegate to track changes to the text itself and to the current selection.

For information about the methods implemented by the delegate, see UITextViewDelegate.

## See Also

### Responding to text view changes

protocol UITextViewDelegate

The methods for receiving editing-related messages for text view objects.

