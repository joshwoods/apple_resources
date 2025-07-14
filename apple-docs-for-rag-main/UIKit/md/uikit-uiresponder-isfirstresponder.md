

- UIKit
- UIResponder
-  isFirstResponder 

Instance Property

# isFirstResponder

Returns a Boolean value indicating whether this object is the first responder.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isFirstResponder: Bool { get }
```

## Return Value

true if the responder is the first responder; otherwise, false.

## Discussion

UIKit dispatches some types of events, such as motion events, to the first responder initially.

## See Also

### Managing the responder chain

var next: UIResponder?

Returns the next responder in the responder chain, or `nil` if there’s no next responder.

var canBecomeFirstResponder: Bool

Returns a Boolean value indicating whether this object can become the first responder.

func becomeFirstResponder() -> Bool

Asks UIKit to make this object the first responder in its window.

var canResignFirstResponder: Bool

Returns a Boolean value indicating whether the responder is willing to relinquish first-responder status.

func resignFirstResponder() -> Bool

Notifies this object that it has been asked to relinquish its status as first responder in its window.

