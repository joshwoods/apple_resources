

- TVUIKit
- TVMediaItemContentConfiguration
-  image 

Instance Property

# image

The image to display.

tvOS 15.0+

``` source
var image: UIImage? { get set }
```

## See Also

### Customizing Content

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

var playbackProgress: Float

The playback progress to display for the media item.

