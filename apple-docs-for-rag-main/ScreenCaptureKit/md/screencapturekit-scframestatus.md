

- ScreenCaptureKit
-  SCFrameStatus 

Enumeration

# SCFrameStatus

Status values for a frame from a stream.

Mac Catalyst 18.2+macOS 12.3+

``` source
enum SCFrameStatus
```

## Overview

You create a frame status by initializing it with the value you retrieve for the status from the sample buffer’s attachments dictionary.

```
if let statusRawValue = attachments[SCStreamFrameInfo.status] as? Int {
    // Create status value.
    let status = SCFrameStatus(rawValue: statusRawValue)
    ...
}
```

## Topics

### Status values

case complete

A status that indicates the system successfully generated a new frame.

case idle

A status that indicates the system didn’t generate a new frame because the display didn’t change.

case blank

A status that indicates the system didn’t generate a new frame because the display is blank.

case started

A status that indicates the frame is the first one sent after the stream starts.

case suspended

A status that indicates the system didn’t generate a new frame because you suspended updates.

case stopped

A status that indicates the frame is in a stopped state.

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

### Output processing

protocol SCStreamOutput

A delegate protocol your app implements to receive capture stream output events.

enum SCStreamOutputType

Constants that represent output types for a stream frame.

struct SCStreamFrameInfo

An instance that defines metadata keys for a stream frame.

