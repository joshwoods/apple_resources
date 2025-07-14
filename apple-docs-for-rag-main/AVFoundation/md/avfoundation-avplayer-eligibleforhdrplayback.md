

- AVFoundation
- AVPlayer
-  eligibleForHDRPlayback 

Type Property

# eligibleForHDRPlayback

A Boolean value that indicates whether the current device can present content to an HDR display.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+tvOS 13.4+visionOS 1.0+

``` source
nonisolated
class var eligibleForHDRPlayback: Bool { get }
```

## Discussion

This property is not key-value observable.

## See Also

### Determining HDR Playback Eligibility

class var availableHDRModes: AVPlayer.HDRMode

The HDR modes that are available for playback.

struct HDRMode

A bitfield type that specifies an HDR mode.

class let eligibleForHDRPlaybackDidChangeNotification: NSNotification.Name

A notification that’s posted whenever HDR playback eligibility changes.

