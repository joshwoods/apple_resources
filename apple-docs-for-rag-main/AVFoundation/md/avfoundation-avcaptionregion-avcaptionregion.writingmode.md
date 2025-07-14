

- AVFoundation
- AVCaptionRegion
-  AVCaptionRegion.WritingMode 

Enumeration

# AVCaptionRegion.WritingMode

Constants that indicate the writing mode for a region.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum WritingMode
```

## Topics

### Writing Modes

case leftToRightAndTopToBottom

A left-to-right and top-to-bottom writing mode.

case topToBottomAndRightToLeft

A top-to-bottom and right-to-left writing mode.

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

### Accessing the Writing Mode

var writingMode: AVCaptionRegion.WritingMode

The block and inline progression direction of the region.

