

- UIKit
- UIView
-  willRemoveSubview(\_:) 

Instance Method

# willRemoveSubview(\_:)

Tells the view that a subview is about to be removed.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func willRemoveSubview(_ subview: UIView)
```

## Parameters 

`subview`  

The subview that will be removed.

## Discussion

The default implementation of this method does nothing. Subclasses can override it to perform additional actions whenever subviews are removed. This method is called when the subview’s superview changes or when the subview is removed from the view hierarchy completely.

## See Also

### Related Documentation

func removeFromSuperview()

Unlinks the view from its superview and its window, and removes it from the responder chain.

### Observing view-related changes

func didAddSubview(UIView)

Tells the view that a subview was added.

func willMove(toSuperview: UIView?)

Tells the view that its superview is about to change to the specified superview.

func didMoveToSuperview()

Tells the view that its superview changed.

func willMove(toWindow: UIWindow?)

Tells the view that its window object is about to change.

func didMoveToWindow()

Tells the view that its window object changed.

