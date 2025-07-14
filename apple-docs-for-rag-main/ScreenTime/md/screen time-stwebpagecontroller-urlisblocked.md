

- Screen Time
- STWebpageController
-  urlIsBlocked 

Instance Property

# urlIsBlocked

A Boolean that indicates whether a parent or guardian has blocked the URL.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
@MainActor
var urlIsBlocked: Bool { get }
```

## Discussion

When a parent or guardian blocks the webpage’s URL, the webpage controller displays a blocking UI and then sets this property to YES.

## See Also

### Instance properties

var suppressUsageRecording: Bool

A Boolean that indicates whether the webpage controller is not recording web usage.

var url: URL?

The URL for the webpage.

var urlIsPictureInPicture: Bool

A Boolean that indicates whether the webpage is currently displaying a floating picture in picture window.

var urlIsPlayingVideo: Bool

A Boolean that indicates whether there are one or more videos currently playing in the webpage.

