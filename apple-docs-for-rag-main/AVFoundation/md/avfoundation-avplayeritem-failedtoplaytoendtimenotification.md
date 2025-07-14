

- AVFoundation
- AVPlayerItem
-  failedToPlayToEndTimeNotification 

Type Property

# failedToPlayToEndTimeNotification

A notification that the system posts when a player item fails to play to its end time.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class let failedToPlayToEndTimeNotification: NSNotification.Name
```

## Discussion

The notification’s object is the player item that finished playing.

Important

The system may post this notification on a thread other than the one you use to register the observer.

## Topics

### Error Keys

let AVPlayerItemFailedToPlayToEndTimeErrorKey: String

The key to retrieve the error object from the notification’s user information dictionary.

## See Also

### Observing Notifications

class let didPlayToEndTimeNotification: NSNotification.Name

A notification the system posts when a player item plays to its end time.

class let timeJumpedNotification: NSNotification.Name

A notification the system posts when a player item’s time changes discontinuously.

class let playbackStalledNotification: NSNotification.Name

A notification the system posts when a player item media doesn’t arrive in time to continue playback.

class let mediaSelectionDidChangeNotification: NSNotification.Name

A notification the player item posts when its media selection changes.

class let recommendedTimeOffsetFromLiveDidChangeNotification: NSNotification.Name

A notification the player item posts when its offset from the live time changes.

class let newAccessLogEntryNotification: NSNotification.Name

A notification the system posts when a player item adds a new entry to its access log.

class let newErrorLogEntryNotification: NSNotification.Name

A notification the system posts when a player item adds a new entry to its error log.

