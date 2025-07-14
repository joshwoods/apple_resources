

- ScreenCaptureKit
-  SCStreamFrameInfo 

Structure

# SCStreamFrameInfo

An instance that defines metadata keys for a stream frame.

Mac Catalyst 18.2+macOS 12.3+

``` source
struct SCStreamFrameInfo
```

## Overview

Use SCStreamFrameInfo keys to retrieve values from the dictionary of metadata attached to the sample buffers that a stream produces. For example, you can retrieve the display time, content scale, and scaling factor, as shown below:

```
// A dictionary of attachments for a streamed sample buffer.
let attachments: [SCStreamFrameInfo: Any] = // Retrieve attachments from a sample buffer.

let displayTime = attachments[.displayTime] as? UInt64 ?? 0
let contentScale = attachments[.contentScale] as? Double ?? 0.0
let scaleFactor = attachments[.scaleFactor] as? Double ?? 0.0
```

## Topics

### Frame information constants

static let status: SCStreamFrameInfo

A key to retrieve the status of a video frame.

static let displayTime: SCStreamFrameInfo

A key to retrieve the display time of a video frame.

static let scaleFactor: SCStreamFrameInfo

A key to retrieve the scale factor of a video frame.

static let contentScale: SCStreamFrameInfo

A key to retrieve the content scale of a video frame.

static let contentRect: SCStreamFrameInfo

A key to retrieve the content rectangle of a video frame.

static let boundingRect: SCStreamFrameInfo

A key to retrieve the bounding rectangle for a video frame.

static let screenRect: SCStreamFrameInfo

A key to retrieve the onscreen location of captured content.

static let dirtyRects: SCStreamFrameInfo

A key to retrieve the areas of a video frame that contain changes.

static let presenterOverlayContentRect: SCStreamFrameInfo

### Initializers

init(rawValue: String)

Creates a new instance with a raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Output processing

protocol SCStreamOutput

A delegate protocol your app implements to receive capture stream output events.

enum SCStreamOutputType

Constants that represent output types for a stream frame.

enum SCFrameStatus

Status values for a frame from a stream.

