

- AVFoundation
-  AVVideoFieldMode 

Enumeration

# AVVideoFieldMode

Constants that indicate which interlacing modes the connection applies to video flowing through it.

macOS 10.7+

``` source
enum AVVideoFieldMode
```

## Overview

The values apply to the videoFieldMode property.

## Topics

### Constants

case both

A value that indicates that a video connection passes both the top and bottom video fields.

case topOnly

A value that indicates that a video connection only passes the top video field.

case bottomOnly

A value that indicates that a video connection only passes the bottom video field.

case deinterlace

A value that indicates that a video connection deinterlaces the top and bottom video fields.

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

### Interlacing video

var isVideoFieldModeSupported: Bool

A Boolean value that indicates whether the connection supports setting a video field mode.

var videoFieldMode: AVVideoFieldMode

A setting that tells the connection how to interlace video flowing through it.

