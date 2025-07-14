

- ScreenCaptureKit
-  SCCaptureResolutionType 

Enumeration

# SCCaptureResolutionType

Available resolutions for content capture.

Mac Catalyst 18.2+macOS 12.3+

``` source
enum SCCaptureResolutionType
```

## Overview

Higher-resolution values produce better and more accurate-looking content to the source, at the expense of bandwidth.

## Topics

### Resolutions

case automatic

Allow ScreenCaptureKit to automatically select the quality of content depending on factors such as network connection.

case best

Capture streaming content at the best available resolution.

case nominal

Capture streaming content with a one point to one pixel conversion factor.

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

### Configuring captured frames

var queueDepth: Int

The maximum number of frames for the queue to store.

var minimumFrameInterval: CMTime

The desired minimum time between frame updates, in seconds.

var captureResolution: SCCaptureResolutionType

The resolution at which to capture source content.

