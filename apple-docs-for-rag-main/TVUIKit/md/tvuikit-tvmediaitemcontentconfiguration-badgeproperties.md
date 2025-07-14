

- TVUIKit
- TVMediaItemContentConfiguration
-  badgeProperties 

Instance Property

# badgeProperties

Properties for configuring the badge.

tvOS 15.0+

``` source
var badgeProperties: TVMediaItemContentConfiguration.BadgeProperties { get set }
```

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

struct BadgeProperties

Properties that affect the media item content badge.

var overlayView: UIView?

An overlay view the system places above the image and automatically resizes to fill the frame.

var playbackProgress: Float

The playback progress to display for the media item.

