

- Foundation
- NSNotification
- NSNotification.Name
-  WKAccessibilityReduceMotionStatusDidChange 

Type Property

# WKAccessibilityReduceMotionStatusDidChange

Tells the interface controller that the reduce motion status has changed.

watchOS 4.0+

``` source
static let WKAccessibilityReduceMotionStatusDidChange: NSNotification.Name
```

## Discussion

Use this notification to customize your application’s user interface for when reduced motion is enabled. You can also use the WKAccessibilityIsReduceMotionEnabled() function to determine whether reduced motion is enabled.

Observe this notification using the default notification center. This notification doesn’t include a parameter.

## See Also

### WatchKit

static let WKAudioFilePlayerItemDidPlayToEndTime: NSNotification.Name

A notification that the item has played successfully to its end.

Deprecated

static let WKAudioFilePlayerItemFailedToPlayToEndTime: NSNotification.Name

A notification that the item failed to play to its end.

Deprecated

static let WKAudioFilePlayerItemTimeJumped: NSNotification.Name

A notification that the item’s current time has changed discontinuously.

Deprecated

