

- AVFoundation
- AVPlaybackCoordinator
-  suspensionReasonsDidChangeNotification 

Type Property

# suspensionReasonsDidChangeNotification

A notification that the coordinator posts when its suspension reasons change.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class let suspensionReasonsDidChangeNotification: NSNotification.Name
```

## See Also

### Observing Suspension Reasons

var suspensionReasons: [AVCoordinatedPlaybackSuspension.Reason]

The reasons a coordinator is currently unable to participate in a group playback activity.

