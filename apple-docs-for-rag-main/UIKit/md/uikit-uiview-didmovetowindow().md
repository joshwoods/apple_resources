

- UIKit
- UIView
-  didMoveToWindow() 

Instance Method

# didMoveToWindow()

Tells the view that its window object changed.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func didMoveToWindow()
```

## Discussion

The default implementation of this method does nothing. Subclasses can override it to perform additional actions whenever the window changes.

The window property may be `nil` by the time that this method is called, indicating that the receiver does not currently reside in any window. This occurs when the receiver has just been removed from its superview or when the receiver has just been added to a superview that is not attached to a window. Overrides of this method may choose to ignore such cases if they are not of interest.

## See Also

### Observing view-related changes

func didAddSubview(UIView)

Tells the view that a subview was added.

func willRemoveSubview(UIView)

Tells the view that a subview is about to be removed.

func willMove(toSuperview: UIView?)

Tells the view that its superview is about to change to the specified superview.

func didMoveToSuperview()

Tells the view that its superview changed.

func willMove(toWindow: UIWindow?)

Tells the view that its window object is about to change.

