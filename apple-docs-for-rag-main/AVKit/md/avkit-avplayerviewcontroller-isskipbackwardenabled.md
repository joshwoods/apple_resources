

- AVKit
- AVPlayerViewController
-  isSkipBackwardEnabled 

Instance Property

# isSkipBackwardEnabled

A Boolean value that indicates whether backward-skipping is available.

tvOS 10.0+

``` source
@MainActor
var isSkipBackwardEnabled: Bool { get set }
```

## Discussion

This property affects the appearance of the backward-skipping indicator. The value you set for the player view controller’s skippingBehavior property determines its backward-skipping behavior.

## See Also

### Configuring Skipping Behavior

var isSkipForwardEnabled: Bool

A Boolean value that indicates whether forward-skipping is available.

var skippingBehavior: AVPlayerViewControllerSkippingBehavior

The behavior that skipping gestures perform.

enum AVPlayerViewControllerSkippingBehavior

Constants that represent the player view controller’s skipping behavior.

