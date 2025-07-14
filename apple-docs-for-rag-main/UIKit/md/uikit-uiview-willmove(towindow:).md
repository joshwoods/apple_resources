

- UIKit
- UIView
-  willMove(toWindow:) 

Instance Method

# willMove(toWindow:)

Tells the view that its window object is about to change.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func willMove(toWindow newWindow: UIWindow?)
```

## Parameters 

`newWindow`  

The window object that will be at the root of the receiver’s new view hierarchy. This parameter may be `nil`.

## Discussion

The default implementation of this method does nothing. Subclasses can override it to perform additional actions whenever the window changes.

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

func didMoveToWindow()

Tells the view that its window object changed.

