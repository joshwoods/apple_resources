

- UIKit
- UIEvent
-  touches(for:) 

Instance Method

# touches(for:)

Returns the touch objects that are being delivered to the specified gesture recognizer.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func touches(for gesture: UIGestureRecognizer) -> Set?
```

## Parameters 

`gesture`  

An instance of a subclass of the abstract base class UIGestureRecognizer. This gesture-recognizer object must be attached to a view to receive the touches hit-tested to that view and its subviews.

## Return Value

A set of UITouch objects representing the touches being delivered to the specified gesture recognizer for the event represented by the receiver.

