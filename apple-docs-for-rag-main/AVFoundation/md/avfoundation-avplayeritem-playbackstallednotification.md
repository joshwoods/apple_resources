

- AVFoundation
- AVPlayerItem
-  playbackStalledNotification 

Type Property

# playbackStalledNotification

A notification the system posts when a player item media doesn’t arrive in time to continue playback.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class let playbackStalledNotification: NSNotification.Name
```

## Discussion

The notification’s object is the player item whose playback is unable to continue due to network delays. Streaming-media playback continues after the player item retrieves a sufficient amount of data. File-based playback doesn’t continue.

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

class let mediaSelectionDidChangeNotification: NSNotification.Name

A notification the player item posts when its media selection changes.

class let recommendedTimeOffsetFromLiveDidChangeNotification: NSNotification.Name

A notification the player item posts when its offset from the live time changes.

class let newAccessLogEntryNotification: NSNotification.Name

A notification the system posts when a player item adds a new entry to its access log.

class let newErrorLogEntryNotification: NSNotification.Name

A notification the system posts when a player item adds a new entry to its error log.

