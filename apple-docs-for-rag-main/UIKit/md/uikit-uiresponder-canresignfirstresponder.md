

- UIKit
- UIResponder
-  canResignFirstResponder 

Instance Property

# canResignFirstResponder

Returns a Boolean value indicating whether the responder is willing to relinquish first-responder status.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var canResignFirstResponder: Bool { get }
```

## Return Value

true if the responder can resign first-responder status; otherwise, false.

## Discussion

This method returns true by default. You can override this method in your custom responders and return a different value if needed. For example, a text field containing invalid content might want to return false to ensure that the user corrects that content first.

## See Also

### Managing the responder chain

var next: UIResponder?

Returns the next responder in the responder chain, or `nil` if there’s no next responder.

var isFirstResponder: Bool

Returns a Boolean value indicating whether this object is the first responder.

var canBecomeFirstResponder: Bool

Returns a Boolean value indicating whether this object can become the first responder.

func becomeFirstResponder() -> Bool

Asks UIKit to make this object the first responder in its window.

func resignFirstResponder() -> Bool

Notifies this object that it has been asked to relinquish its status as first responder in its window.

