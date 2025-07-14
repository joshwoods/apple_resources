

- Metal
-  MTLCaptureDescriptor 

Class

# MTLCaptureDescriptor

A configuration for a Metal capture session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MTLCaptureDescriptor
```

## Topics

### Setting Capture Parameters

var captureObject: Any?

The object whose contents should be captured.

var destination: MTLCaptureDestination

The destination for any captured command data.

var outputURL: URL?

A URL for a file to write the capture data into.

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

## See Also

### Frame Capture

class MTLCaptureManager

An instance you use to capture Metal command data in your app.

enum MTLCaptureDestination

The kinds of destinations for captured command data.

protocol MTLCaptureScope

A protocol that defines custom boundaries for a GPU frame capture.

