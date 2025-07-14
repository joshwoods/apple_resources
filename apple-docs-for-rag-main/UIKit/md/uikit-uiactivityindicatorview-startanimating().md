

- UIKit
- UIActivityIndicatorView
-  startAnimating() 

Instance Method

# startAnimating()

Starts the animation of the progress indicator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func startAnimating()
```

## Discussion

When the progress indicator is animated, the gear spins to indicate indeterminate progress. The indicator is animated until stopAnimating() is called.

## See Also

### Managing an activity indicator

func stopAnimating()

Stops the animation of the progress indicator.

var isAnimating: Bool

A Boolean value indicating whether the activity indicator is currently running its animation.

var hidesWhenStopped: Bool

A Boolean value that controls whether the activity indicator is hidden when the animation is stopped.

