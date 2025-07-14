

- AVFoundation
- AVPlayer
-  eligibleForHDRPlaybackDidChangeNotification 

Type Property

# eligibleForHDRPlaybackDidChangeNotification

A notification that’s posted whenever HDR playback eligibility changes.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+tvOS 13.4+visionOS 1.0+

``` source
class let eligibleForHDRPlaybackDidChangeNotification: NSNotification.Name
```

## Discussion

The system may post this notification if a user connects or disconnects a display, or makes other system resource changes.

## See Also

### Determining HDR Playback Eligibility

class var eligibleForHDRPlayback: Bool

A Boolean value that indicates whether the current device can present content to an HDR display.

class var availableHDRModes: AVPlayer.HDRMode

The HDR modes that are available for playback.

struct HDRMode

A bitfield type that specifies an HDR mode.

