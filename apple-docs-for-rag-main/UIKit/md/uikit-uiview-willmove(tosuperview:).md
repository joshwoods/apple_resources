

- UIKit
- UIView
-  willMove(toSuperview:) 

Instance Method

# willMove(toSuperview:)

Tells the view that its superview is about to change to the specified superview.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func willMove(toSuperview newSuperview: UIView?)
```

## Parameters 

`newSuperview`  

A view object that will be the new superview of the receiver. This object may be `nil`.

## Discussion

The default implementation of this method does nothing. Subclasses can override it to perform additional actions whenever the superview changes.

## See Also

### Observing view-related changes

func didAddSubview(UIView)

Tells the view that a subview was added.

func willRemoveSubview(UIView)

Tells the view that a subview is about to be removed.

func didMoveToSuperview()

Tells the view that its superview changed.

func willMove(toWindow: UIWindow?)

Tells the view that its window object is about to change.

func didMoveToWindow()

Tells the view that its window object changed.

