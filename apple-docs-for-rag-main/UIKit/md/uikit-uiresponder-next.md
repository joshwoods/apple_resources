

- UIKit
- UIResponder
-  next 

Instance Property

# next

Returns the next responder in the responder chain, or `nil` if there’s no next responder.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var next: UIResponder? { get }
```

## Return Value

The next object in the responder chain, or `nil` if this is the last object in the chain.

## Mentioned in 

Using responders and the responder chain to handle events

## Discussion

The UIResponder class doesn’t store or set the next responder automatically, so this method returns `nil` by default. Subclasses must override this method and return an appropriate next responder. For example, UIView implements this method and returns the UIViewController object that manages it (if it has one) or its superview (if it doesn’t). UIViewController similarly implements the method and returns its view’s superview. UIWindow returns the application object. The shared UIApplication object normally returns `nil`, but it returns its app delegate if that object is a subclass of UIResponder and hasn’t already been called to handle the event.

## See Also

### Managing the responder chain

var isFirstResponder: Bool

Returns a Boolean value indicating whether this object is the first responder.

var canBecomeFirstResponder: Bool

Returns a Boolean value indicating whether this object can become the first responder.

func becomeFirstResponder() -> Bool

Asks UIKit to make this object the first responder in its window.

var canResignFirstResponder: Bool

Returns a Boolean value indicating whether the responder is willing to relinquish first-responder status.

func resignFirstResponder() -> Bool

Notifies this object that it has been asked to relinquish its status as first responder in its window.

