

- UIKit
- UIView
-  didMoveToSuperview() 

Instance Method

# didMoveToSuperview()

Tells the view that its superview changed.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func didMoveToSuperview()
```

## Discussion

The default implementation of this method does nothing. Subclasses can override it to perform additional actions whenever the superview changes.

## See Also

### Observing view-related changes

func didAddSubview(UIView)

Tells the view that a subview was added.

func willRemoveSubview(UIView)

Tells the view that a subview is about to be removed.

func willMove(toSuperview: UIView?)

Tells the view that its superview is about to change to the specified superview.

func willMove(toWindow: UIWindow?)

Tells the view that its window object is about to change.

func didMoveToWindow()

Tells the view that its window object changed.

