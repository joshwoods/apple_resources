

- AVFoundation
- AVCoordinatedPlaybackSuspension
-  reason 

Instance Property

# reason

The reason for the suspension.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var reason: AVCoordinatedPlaybackSuspension.Reason { get }
```

## Discussion

The coordinator communicates the suspension reason to other participants.

## See Also

### Inspecting a Suspension

var beginDate: Date

The time the suspension begins.

struct Reason

Constants that identify playback suspension reasons.

