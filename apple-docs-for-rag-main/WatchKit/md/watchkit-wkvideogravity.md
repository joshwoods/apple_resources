

- WatchKit
-  WKVideoGravity 

Enumeration

# WKVideoGravity

Constants indicating the appearance of video content.

watchOS 2.0+

``` source
enum WKVideoGravity
```

## Topics

### Constants

case resizeAspect

Content is resized to fit the bounds rectangle, preserving the original aspect ratio of the content. Content that does not completely fill the bounds rectangle is centered in the partial axis.

case resizeAspectFill

Content is resized to fill the bounds rectangle completely while preserving the original aspect ratio of the content. This option results in cropping of the edges of the video in the axis it exceeds.

case resize

Content is resized to fit the entire bounds rectangle. This option does not preserve the original aspect ratio of the content.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Images and movies

class WKInterfaceImage

An image that can be displayed in the interface of your watchOS app.

class WKImage

A wrapper for images you use with a picker interface.

protocol WKImageAnimatable

A collection of methods you can use to control the playback of animated images.

class WKInterfaceMovie

An interface element that lets you play video and audio content in your watchOS app.

class WKInterfaceInlineMovie

An interface element that displays a video’s poster image and supports inline playing of the video.

class WKInterfaceHMCamera

An interface element that displays either a video stream or a single snapshot from an IP camera connected to HomeKit.

