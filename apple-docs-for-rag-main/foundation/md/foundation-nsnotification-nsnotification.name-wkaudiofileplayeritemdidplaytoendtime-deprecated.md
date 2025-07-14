

- Foundation
- NSNotification
- NSNotification.Name
-  WKAudioFilePlayerItemDidPlayToEndTime Deprecated

Type Property

# WKAudioFilePlayerItemDidPlayToEndTime

A notification that the item has played successfully to its end.

watchOS 2.0–6.0Deprecated

``` source
static let WKAudioFilePlayerItemDidPlayToEndTime: NSNotification.Name
```

Deprecated

Use the AVFoundation framework’s AVPlayer and AVQueuePlayer classes instead.

## Discussion

The notification’s object is the player item. There is no `userInfo` dictionary.

## See Also

### WatchKit

static let WKAccessibilityReduceMotionStatusDidChange: NSNotification.Name

Tells the interface controller that the reduce motion status has changed.

static let WKAudioFilePlayerItemFailedToPlayToEndTime: NSNotification.Name

A notification that the item failed to play to its end.

Deprecated

static let WKAudioFilePlayerItemTimeJumped: NSNotification.Name

A notification that the item’s current time has changed discontinuously.

Deprecated

