

- AVFoundation
- AVPlayerItem
-  newAccessLogEntryNotification 

Type Property

# newAccessLogEntryNotification

A notification the system posts when a player item adds a new entry to its access log.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class let newAccessLogEntryNotification: NSNotification.Name
```

## Discussion

The notification’s object is the player item.

Important

The system may post this notification on a thread other than the one you use to register the observer.

## See Also

### Observing Notifications

class let didPlayToEndTimeNotification: NSNotification.Name

A notification the system posts when a player item plays to its end time.

class let failedToPlayToEndTimeNotification: NSNotification.Name

A notification that the system posts when a player item fails to play to its end time.

class let timeJumpedNotification: NSNotification.Name

A notification the system posts when a player item’s time changes discontinuously.

class let playbackStalledNotification: NSNotification.Name

A notification the system posts when a player item media doesn’t arrive in time to continue playback.

class let mediaSelectionDidChangeNotification: NSNotification.Name

A notification the player item posts when its media selection changes.

class let recommendedTimeOffsetFromLiveDidChangeNotification: NSNotification.Name

A notification the player item posts when its offset from the live time changes.

class let newErrorLogEntryNotification: NSNotification.Name

A notification the system posts when a player item adds a new entry to its error log.

