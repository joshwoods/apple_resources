

- AVFoundation
- AVPlaybackCoordinator
-  suspensionReasons 

Instance Property

# suspensionReasons

The reasons a coordinator is currently unable to participate in a group playback activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var suspensionReasons: [AVCoordinatedPlaybackSuspension.Reason] { get }
```

## Discussion

The coordinator doesn’t respond to changes in group playback state when this property value contains suspension reasons.

Note

To observe changes to this property value, register for notifications of type suspensionReasonsDidChangeNotification.

## See Also

### Observing Suspension Reasons

class let suspensionReasonsDidChangeNotification: NSNotification.Name

A notification that the coordinator posts when its suspension reasons change.

