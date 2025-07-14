

- AVKit
- AVPlayerViewController
-  isSkipForwardEnabled 

Instance Property

# isSkipForwardEnabled

A Boolean value that indicates whether forward-skipping is available.

tvOS 10.0+

``` source
@MainActor
var isSkipForwardEnabled: Bool { get set }
```

## Discussion

This property affects the appearance of the forward-skipping indicator. The value you set for the player view controller’s skippingBehavior property determines its forward-skipping behavior.

## See Also

### Configuring Skipping Behavior

var isSkipBackwardEnabled: Bool

A Boolean value that indicates whether backward-skipping is available.

var skippingBehavior: AVPlayerViewControllerSkippingBehavior

The behavior that skipping gestures perform.

enum AVPlayerViewControllerSkippingBehavior

Constants that represent the player view controller’s skipping behavior.

