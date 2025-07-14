

- Core Video
-  CVAttachmentMode 

Enumeration

# CVAttachmentMode

The propagation modes of a Core Video buffer attachment.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
enum CVAttachmentMode
```

## Overview

You set these attributes when adding attachments to a CVBuffer object.

## Topics

### Constants

case shouldNotPropagate

Indicates to not propagate the attachment.

case shouldPropagate

Indicates to copy the attachment.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Data types

class CVBuffer

A reference to a Core Video buffer.

