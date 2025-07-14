

- UIKit
- UIView
-  didAddSubview(\_:) 

Instance Method

# didAddSubview(\_:)

Tells the view that a subview was added.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func didAddSubview(_ subview: UIView)
```

## Parameters 

`subview`  

The view that was added as a subview.

## Discussion

The default implementation of this method does nothing. Subclasses can override it to perform additional actions when subviews are added. This method is called in response to adding a subview using any of the relevant view methods.

## See Also

### Related Documentation

func insertSubview(UIView, belowSubview: UIView)

Inserts a view below another view in the view hierarchy.

func insertSubview(UIView, aboveSubview: UIView)

Inserts a view above another view in the view hierarchy.

func addSubview(UIView)

Adds a view to the end of the receiver’s list of subviews.

func insertSubview(UIView, at: Int)

Inserts a subview at the specified index.

### Observing view-related changes

func willRemoveSubview(UIView)

Tells the view that a subview is about to be removed.

func willMove(toSuperview: UIView?)

Tells the view that its superview is about to change to the specified superview.

func didMoveToSuperview()

Tells the view that its superview changed.

func willMove(toWindow: UIWindow?)

Tells the view that its window object is about to change.

func didMoveToWindow()

Tells the view that its window object changed.

