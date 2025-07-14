

- UIKit
- UIActivityIndicatorView
-  hidesWhenStopped 

Instance Property

# hidesWhenStopped

A Boolean value that controls whether the activity indicator is hidden when the animation is stopped.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var hidesWhenStopped: Bool { get set }
```

## Discussion

If the value of this property is true (the default), the receiver sets its isHidden property (`UIView`) to true when receiver is not animating. If the hidesWhenStopped property is false, the receiver is not hidden when animation stops. You stop an animating progress indicator with the stopAnimating() method.

## See Also

### Managing an activity indicator

func startAnimating()

Starts the animation of the progress indicator.

func stopAnimating()

Stops the animation of the progress indicator.

var isAnimating: Bool

A Boolean value indicating whether the activity indicator is currently running its animation.

