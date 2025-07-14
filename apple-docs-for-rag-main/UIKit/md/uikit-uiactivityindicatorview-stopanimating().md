

- UIKit
- UIActivityIndicatorView
-  stopAnimating() 

Instance Method

# stopAnimating()

Stops the animation of the progress indicator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func stopAnimating()
```

## Discussion

Call this method to stop the animation of the progress indicator started with a call to startAnimating(). When animating is stopped, the indicator is hidden, unless hidesWhenStopped is false.

## See Also

### Managing an activity indicator

func startAnimating()

Starts the animation of the progress indicator.

var isAnimating: Bool

A Boolean value indicating whether the activity indicator is currently running its animation.

var hidesWhenStopped: Bool

A Boolean value that controls whether the activity indicator is hidden when the animation is stopped.

