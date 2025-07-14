

- UIKit
- UIView
-  insertSubview(\_:aboveSubview:) 

Instance Method

# insertSubview(\_:aboveSubview:)

Inserts a view above another view in the view hierarchy.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func insertSubview(
    _ view: UIView,
    aboveSubview siblingSubview: UIView
)
```

## Parameters 

`view`  

The view to insert. It’s removed from its superview if it’s not a sibling of `siblingSubview`.

`siblingSubview`  

The sibling view that will be behind the inserted view.

## Discussion

This method establishes a strong reference to `view` and sets its next responder to the receiver, which is its new superview.

Views can have only one superview. If `view` already has a superview and that view is not the receiver, this method removes the previous superview before making the receiver its new superview.

## See Also

### Managing the view hierarchy

var superview: UIView?

The receiver’s superview, or `nil` if it has none.

var subviews: [UIView]

The receiver’s immediate subviews.

var window: UIWindow?

The receiver’s window object, or `nil` if it has none.

func addSubview(UIView)

Adds a view to the end of the receiver’s list of subviews.

func bringSubviewToFront(UIView)

Moves the specified subview so that it appears on top of its siblings.

func sendSubviewToBack(UIView)

Moves the specified subview so that it appears behind its siblings.

func removeFromSuperview()

Unlinks the view from its superview and its window, and removes it from the responder chain.

func insertSubview(UIView, at: Int)

Inserts a subview at the specified index.

func insertSubview(UIView, belowSubview: UIView)

Inserts a view below another view in the view hierarchy.

func exchangeSubview(at: Int, withSubviewAt: Int)

Exchanges the subviews at the specified indices.

func isDescendant(of: UIView) -> Bool

Returns a Boolean value indicating whether the receiver is a subview of a given view or identical to that view.

