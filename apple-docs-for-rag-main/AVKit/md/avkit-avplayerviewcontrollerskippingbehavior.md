

- AVKit
-  AVPlayerViewControllerSkippingBehavior 

Enumeration

# AVPlayerViewControllerSkippingBehavior

Constants that represent the player view controller’s skipping behavior.

tvOS 10.0+

``` source
enum AVPlayerViewControllerSkippingBehavior
```

## Topics

### Skipping Behaviors

case `default`

The default skipping behavior, which is to skip forward or backward in 10-second intervals.

case skipItem

Skipping behavior that specifies skipping to the next or previous item in the player’s playlist.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Skipping Behavior

var isSkipForwardEnabled: Bool

A Boolean value that indicates whether forward-skipping is available.

var isSkipBackwardEnabled: Bool

A Boolean value that indicates whether backward-skipping is available.

var skippingBehavior: AVPlayerViewControllerSkippingBehavior

The behavior that skipping gestures perform.

