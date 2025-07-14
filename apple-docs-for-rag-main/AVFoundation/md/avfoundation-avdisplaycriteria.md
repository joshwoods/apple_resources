

- AVFoundation
-  AVDisplayCriteria 

Class

# AVDisplayCriteria

An object the system uses to guide the selection of a display mode in tvOS.

tvOS 11.2+visionOS 1.0+

``` source
class AVDisplayCriteria
```

## Overview

In tvOS, this object provides the display criteria that an AVDisplayManager uses to set an appropriate display mode, such as switching to HDR, when presenting a video asset. If your app uses AVPlayerViewController for its player user interface, the system automatically applies the display critera when it presents the asset. If you use a custom player interface, load the value of an asset’s preferredDisplayCriteria property and set it on the window’s avDisplayManager object.

Important

Most apps don’t create instances of this class, and instead retrieve the preferred display criteria from a media asset. If your app doesn’t use AVAsset, such as a streaming app that renders sample buffers using AVSampleBufferDisplayLayer, you can manually create an instance using the init(refreshRate:formatDescription:) initializer.

## Topics

### Create a display criteria

init(refreshRate: Float, formatDescription: CMFormatDescription)

Creates a display criteria object with the specified refresh rate and format description.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Loading Asset Preferences

static var preferredRate: AVAsyncProperty&lt;Root, Float>

The asset’s rate preference for playing its media.

static var preferredVolume: AVAsyncProperty&lt;Root, Float>

The asset’s volume preference for playing its audible media.

static var preferredTransform: AVAsyncProperty&lt;Root, CGAffineTransform>

The asset’s transform preference to apply to its visual content during presentation or processing.

static var preferredDisplayCriteria: AVAsyncProperty&lt;Root, AVDisplayCriteria>

The asset’s display mode preference for optimal playback of its content.

