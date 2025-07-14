

- UIKit
- UIView
-  point(inside:with:) 

Instance Method

# point(inside:with:)

Returns a Boolean value indicating whether the receiver contains the specified point.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func point(
    inside point: CGPoint,
    with event: UIEvent?
) -> Bool
```

## Parameters 

`point`  

A point that is in the receiver’s local coordinate system (bounds).

`event`  

The event that warranted a call to this method. If you are calling this method from outside your event-handling code, you may specify `nil`.

## Return Value

true if `point` is inside the receiver’s bounds; otherwise, false.

## See Also

### Hit-testing in a view

func hitTest(CGPoint, with: UIEvent?) -> UIView?

Returns the farthest descendant in the view hierarchy of the current view, including itself, that contains the specified point.

