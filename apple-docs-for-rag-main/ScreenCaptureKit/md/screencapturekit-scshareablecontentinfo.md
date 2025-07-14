

- ScreenCaptureKit
-  SCShareableContentInfo 

Class

# SCShareableContentInfo

An instance that provides information for the content in a given stream.

Mac Catalyst 18.2+macOS 14.0+

``` source
class SCShareableContentInfo
```

## Topics

### Shared content properties

var contentRect: CGRect

The size and location of content for the stream.

var pointPixelScale: Float

The scaling from points to output pixel resolution for the stream.

var style: SCShareableContentStyle

The current presentation style of the stream.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Shareable content

class SCShareableContent

An instance that represents a set of displays, apps, and windows that your app can capture.

enum SCShareableContentStyle

The style of content presented in a stream.

class SCDisplay

An instance that represents a display device.

class SCRunningApplication

An instance that represents an app running on a device.

class SCWindow

An instance that represents an onscreen window.

