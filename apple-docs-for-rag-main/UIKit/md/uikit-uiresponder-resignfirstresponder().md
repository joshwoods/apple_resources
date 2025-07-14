

- UIKit
- UIResponder
-  resignFirstResponder() 

Instance Method

# resignFirstResponder()

Notifies this object that it has been asked to relinquish its status as first responder in its window.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func resignFirstResponder() -> Bool
```

## Discussion

The default implementation returns true, resigning first responder status. You can override this method in your custom responders to update your object’s state or perform other actions, such as removing the highlight from a selection. You can also return false, refusing to relinquish first responder status. If you override this method, you must call `super` (the superclass implementation) at some point in your code.

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

var canResignFirstResponder: Bool

Returns a Boolean value indicating whether the responder is willing to relinquish first-responder status.

