

- AVFoundation
- AVPlayerItemIntegratedTimeline
-  currentDate 

Instance Property

# currentDate

The current date of playback.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var currentDate: Date? { get }
```

## Discussion

This value is `nil` if playback doesn’t map to a date.

## See Also

### Inspecting the time and date

var currentTime: CMTime

The current time on the integrated timeline.

