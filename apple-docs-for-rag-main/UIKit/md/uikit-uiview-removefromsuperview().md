

- UIKit
- UIView
-  removeFromSuperview() 

Instance Method

# removeFromSuperview()

Unlinks the view from its superview and its window, and removes it from the responder chain.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func removeFromSuperview()
```

## Mentioned in 

Creating a custom container view controller

## Discussion

If the view’s superview is not `nil`, the superview releases the view.

Calling this method removes any constraints that refer to the view you are removing, or that refer to any view in the subtree of the view you are removing.

Important

Never call this method from inside your view’s draw(_:) method.

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

func insertSubview(UIView, at: Int)

Inserts a subview at the specified index.

func insertSubview(UIView, aboveSubview: UIView)

Inserts a view above another view in the view hierarchy.

func insertSubview(UIView, belowSubview: UIView)

Inserts a view below another view in the view hierarchy.

func exchangeSubview(at: Int, withSubviewAt: Int)

Exchanges the subviews at the specified indices.

func isDescendant(of: UIView) -> Bool

Returns a Boolean value indicating whether the receiver is a subview of a given view or identical to that view.

