

- UIKit
- UIView
-  subviews 

Instance Property

# subviews

The receiver’s immediate subviews.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var subviews: [UIView] { get }
```

## Discussion

You can use this property to retrieve the subviews associated with your custom view hierarchies. The order of the subviews in the array reflects their visible order on the screen, with the view at index 0 being the back-most view.

For complex views declared in UIKit and other system frameworks, any subviews of the view are generally considered private and subject to change at any time. Therefore, you should not attempt to retrieve or modify subviews for these types of system-supplied views. If you do, your code may break during a future system update.

## See Also

### Managing the view hierarchy

var superview: UIView?

The receiver’s superview, or `nil` if it has none.

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

func insertSubview(UIView, aboveSubview: UIView)

Inserts a view above another view in the view hierarchy.

func insertSubview(UIView, belowSubview: UIView)

Inserts a view below another view in the view hierarchy.

func exchangeSubview(at: Int, withSubviewAt: Int)

Exchanges the subviews at the specified indices.

func isDescendant(of: UIView) -> Bool

Returns a Boolean value indicating whether the receiver is a subview of a given view or identical to that view.

