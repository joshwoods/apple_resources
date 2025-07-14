

- Screen Time
- STWebpageController
-  suppressUsageRecording 

Instance Property

# suppressUsageRecording

A Boolean that indicates whether the webpage controller is not recording web usage.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
@MainActor
var suppressUsageRecording: Bool { get set }
```

## Discussion

Set to YES to stop recording and reporting web-usage data.

## See Also

### Instance properties

var url: URL?

The URL for the webpage.

var urlIsBlocked: Bool

A Boolean that indicates whether a parent or guardian has blocked the URL.

var urlIsPictureInPicture: Bool

A Boolean that indicates whether the webpage is currently displaying a floating picture in picture window.

var urlIsPlayingVideo: Bool

A Boolean that indicates whether there are one or more videos currently playing in the webpage.

