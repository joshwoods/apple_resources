

- AVFoundation
- AVPlayerItemIntegratedTimeline
-  currentTime 

Instance Property

# currentTime

The current time on the integrated timeline.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var currentTime: CMTime { get }
```

## Discussion

During playback of interstitial events that occupy a single point, this value doesn’t change.

## See Also

### Inspecting the time and date

var currentDate: Date?

The current date of playback.

