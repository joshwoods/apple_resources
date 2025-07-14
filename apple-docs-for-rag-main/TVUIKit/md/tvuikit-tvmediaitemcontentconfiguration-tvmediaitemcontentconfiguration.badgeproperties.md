

- TVUIKit
- TVMediaItemContentConfiguration
-  TVMediaItemContentConfiguration.BadgeProperties 

Structure

# TVMediaItemContentConfiguration.BadgeProperties

Properties that affect the media item content badge.

tvOS 15.0+

``` source
struct BadgeProperties
```

## Topics

### Creating a Default Configuration

static func `default`() -> TVMediaItemContentConfiguration.BadgeProperties

Creates the default configuration for a badge.

static func liveContent() -> TVMediaItemContentConfiguration.BadgeProperties

Creates the default configuration for a badge representing live content.

### Customizing Content

var font: UIFont

The font for the badge text.

var color: UIColor

The color of the badge text.

var backgroundColor: UIColor

The background tint color of the badge.

var transform: TVMediaItemContentConfiguration.TextProperties.TextTransform

The transform to apply to the text before displaying it.

enum TextTransform

Constants that specify the transform to apply to the text.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable

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

var overlayView: UIView?

An overlay view the system places above the image and automatically resizes to fill the frame.

var playbackProgress: Float

The playback progress to display for the media item.

