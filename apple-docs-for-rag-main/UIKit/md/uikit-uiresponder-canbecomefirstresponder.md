

- UIKit
- UIResponder
-  canBecomeFirstResponder 

Instance Property

# canBecomeFirstResponder

Returns a Boolean value indicating whether this object can become the first responder.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var canBecomeFirstResponder: Bool { get }
```

## Return Value

true if the responder can become the first responder; otherwise, false.

## Discussion

This method returns false by default. Subclasses must override this method and return true to be able to become first responder.

Don’t call this method on a view that’s not currently in the active view hierarchy. The result is undefined.

## See Also

### Managing the responder chain

var next: UIResponder?

Returns the next responder in the responder chain, or `nil` if there’s no next responder.

var isFirstResponder: Bool

Returns a Boolean value indicating whether this object is the first responder.

func becomeFirstResponder() -> Bool

Asks UIKit to make this object the first responder in its window.

var canResignFirstResponder: Bool

Returns a Boolean value indicating whether the responder is willing to relinquish first-responder status.

func resignFirstResponder() -> Bool

Notifies this object that it has been asked to relinquish its status as first responder in its window.

