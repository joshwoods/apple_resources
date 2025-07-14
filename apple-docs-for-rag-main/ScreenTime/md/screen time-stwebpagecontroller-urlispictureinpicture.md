

- Screen Time
- STWebpageController
-  urlIsPictureInPicture 

Instance Property

# urlIsPictureInPicture

A Boolean that indicates whether the webpage is currently displaying a floating picture in picture window.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
@MainActor
var urlIsPictureInPicture: Bool { get set }
```

## Discussion

The default value is NO. Set this value when the webpage starts or stops displaying a Picture in Picture window.

Important

Set this value to NO prior to changing url if the new webpage at that URL ends all currently displayed Picture in Picture windows, and won’t immediately display a new one.

## See Also

### Instance properties

var suppressUsageRecording: Bool

A Boolean that indicates whether the webpage controller is not recording web usage.

var url: URL?

The URL for the webpage.

var urlIsBlocked: Bool

A Boolean that indicates whether a parent or guardian has blocked the URL.

var urlIsPlayingVideo: Bool

A Boolean that indicates whether there are one or more videos currently playing in the webpage.

