

- AVFoundation
- AVPlayerItem
-  mediaSelectionDidChangeNotification 

Type Property

# mediaSelectionDidChangeNotification

A notification the player item posts when its media selection changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class let mediaSelectionDidChangeNotification: NSNotification.Name
```

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

class let recommendedTimeOffsetFromLiveDidChangeNotification: NSNotification.Name

A notification the player item posts when its offset from the live time changes.

class let newAccessLogEntryNotification: NSNotification.Name

A notification the system posts when a player item adds a new entry to its access log.

class let newErrorLogEntryNotification: NSNotification.Name

A notification the system posts when a player item adds a new entry to its error log.

