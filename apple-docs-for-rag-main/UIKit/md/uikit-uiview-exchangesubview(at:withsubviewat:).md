

- UIKit
- UIView
-  exchangeSubview(at:withSubviewAt:) 

Instance Method

# exchangeSubview(at:withSubviewAt:)

Exchanges the subviews at the specified indices.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func exchangeSubview(
    at index1: Int,
    withSubviewAt index2: Int
)
```

## Parameters 

`index1`  

The index of the first subview in the receiver.

`index2`  

The index of the second subview in the receiver.

## Discussion

Each index represents the position of the corresponding view in the array in the subviews property. Subview indices start at `0` and cannot be greater than the number of subviews. This method does not change the superview of either view but simply swaps their positions in the subviews array.

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

func insertSubview(UIView, aboveSubview: UIView)

Inserts a view above another view in the view hierarchy.

func insertSubview(UIView, belowSubview: UIView)

Inserts a view below another view in the view hierarchy.

func isDescendant(of: UIView) -> Bool

Returns a Boolean value indicating whether the receiver is a subview of a given view or identical to that view.

