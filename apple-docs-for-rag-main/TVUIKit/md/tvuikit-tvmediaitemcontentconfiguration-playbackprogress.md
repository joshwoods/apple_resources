

- TVUIKit
- TVMediaItemContentConfiguration
-  playbackProgress 

Instance Property

# playbackProgress

The playback progress to display for the media item.

tvOS 15.0+

``` source
var playbackProgress: Float { get set }
```

## Discussion

The system clamps the value between `0.0` and `1.0`.

## See Also

### Customizing Content

var image: UIImage?

The image to display.

var text: String?

The primary text.

var secondaryText: String?

The secondary text.

var badgeText: String?

The text to display in a badge in the top corner of the content.

var badgeProperties: TVMediaItemContentConfiguration.BadgeProperties

Properties for configuring the badge.

struct BadgeProperties

Properties that affect the media item content badge.

var overlayView: UIView?

An overlay view the system places above the image and automatically resizes to fill the frame.

