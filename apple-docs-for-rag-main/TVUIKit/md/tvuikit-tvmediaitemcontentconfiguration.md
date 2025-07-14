

- TVUIKit
-  TVMediaItemContentConfiguration 

Structure

# TVMediaItemContentConfiguration

A content configuration for a media item view.

tvOS 15.0+

``` source
struct TVMediaItemContentConfiguration
```

## Topics

### Creating Default Configurations

static func wideCell() -> TVMediaItemContentConfiguration

Creates the default configuration for a wide media item cell.

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

var playbackProgress: Float

The playback progress to display for the media item.

### Customizing Appearance

struct TextProperties

Properties that affect the media item content configuration’s text.

var textProperties: TVMediaItemContentConfiguration.TextProperties

Properties for configuring the primary text.

var secondaryTextProperties: TVMediaItemContentConfiguration.TextProperties

Properties for configuring the secondary text.

### Creating a Content View

func makeContentView() -> any UIView &amp; UIContentView

Creates a new instance of the content view using this configuration.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- UIContentConfiguration

## See Also

### Creating a Media Item Content View

convenience init(configuration: TVMediaItemContentConfiguration)

Creates a media item content view with the configuration you specify.

