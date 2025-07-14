

- AVKit
- AVPlayerViewController
-  skippingBehavior 

Instance Property

# skippingBehavior

The behavior that skipping gestures perform.

tvOS 10.0+

``` source
@MainActor
var skippingBehavior: AVPlayerViewControllerSkippingBehavior { get set }
```

## Discussion

This property lets you override the default skipping behavior in tvOS, which is to skip forward or backward 10 seconds when a user presses the right or left sides, respectively, of the Touch surface on the Siri Remote.

## See Also

### Configuring Skipping Behavior

var isSkipForwardEnabled: Bool

A Boolean value that indicates whether forward-skipping is available.

var isSkipBackwardEnabled: Bool

A Boolean value that indicates whether backward-skipping is available.

enum AVPlayerViewControllerSkippingBehavior

Constants that represent the player view controller’s skipping behavior.

