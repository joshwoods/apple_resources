

- ScreenCaptureKit
-  SCScreenshotManager 

Class

# SCScreenshotManager

An instance for the capture of single frames from a stream.

Mac Catalyst 18.2+macOS 14.0+

``` source
class SCScreenshotManager
```

## Topics

### Individual frame capture

class func captureImage(contentFilter: SCContentFilter, configuration: SCStreamConfiguration, completionHandler: ((CGImage?, (any Error)?) -> Void)?)

Captures a single frame from a stream as an image, using a filter.

class func captureSampleBuffer(contentFilter: SCContentFilter, configuration: SCStreamConfiguration, completionHandler: ((CMSampleBuffer?, (any Error)?) -> Void)?)

Captures a single frame directly from a stream’s buffer, using a filter.

### Type Methods

class func captureImage(in: CGRect, completionHandler: ((CGImage?, (any Error)?) -> Void)?)

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

### Content capture

class SCStream

An instance that represents a stream of shareable content.

class SCStreamConfiguration

An instance that provides the output configuration for a stream.

class SCContentFilter

An instance that filters the content a stream captures.

protocol SCStreamDelegate

A delegate protocol your app implements to respond to stream events.

