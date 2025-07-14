

- UIKit
- UIView
-  hitTest(\_:with:) 

Instance Method

# hitTest(\_:with:)

Returns the farthest descendant in the view hierarchy of the current view, including itself, that contains the specified point.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func hitTest(
    _ point: CGPoint,
    with event: UIEvent?
) -> UIView?
```

## Parameters 

`point`  

A point in the view’s local coordinate system.

`event`  

The event that warrants a call to this method. If you’re calling this method from outside your event-handling code, you can specify `nil`.

## Return Value

The view object that’s the farthest descendent of the current view and contains `point`. Returns `nil` if the point lies completely outside the view hierarchy of the current view.

## Mentioned in 

Using responders and the responder chain to handle events

## Discussion

This method traverses the view hierarchy by calling the point(inside:with:) method of each subview to determine which subview to send a touch event to. If point(inside:with:) returns true, this method continues to traverse the subview hierarchy until it finds the frontmost view that contains the specified point. If a view doesn’t contain the point, this method ignores its branch of the view hierarchy. You rarely need to call this method yourself, but you might override it to hide touch events from subviews.

This method ignores view objects that are hidden, that have disabled user interactions, or that have an alpha level less than `0.01`. This method doesn’t take the view’s content into account when determining a hit, so it can return a view even if the specified point is in a transparent portion of that view’s content.

This method doesn’t report points that lie outside the view’s bounds as hits, even if they actually lie within one of the view’s subviews. This situation can occur if the view’s clipsToBounds property is false and the affected subview extends beyond the view’s bounds.

Note

When the system calls this method to perform hit-testing for event routing, it expects the resulting view to be part of a UIWindow hierarchy.

## See Also

### Hit-testing in a view

func point(inside: CGPoint, with: UIEvent?) -> Bool

Returns a Boolean value indicating whether the receiver contains the specified point.

