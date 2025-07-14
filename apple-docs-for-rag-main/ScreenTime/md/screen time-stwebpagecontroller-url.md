

- Screen Time
- STWebpageController
-  url 

Instance Property

# url

The URL for the webpage.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
@MainActor
var url: URL? { get set }
```

## Discussion

Set this value to the webpage’s URL when the user navigates to a new URL.

## See Also

### Instance properties

var suppressUsageRecording: Bool

A Boolean that indicates whether the webpage controller is not recording web usage.

var urlIsBlocked: Bool

A Boolean that indicates whether a parent or guardian has blocked the URL.

var urlIsPictureInPicture: Bool

A Boolean that indicates whether the webpage is currently displaying a floating picture in picture window.

var urlIsPlayingVideo: Bool

A Boolean that indicates whether there are one or more videos currently playing in the webpage.

