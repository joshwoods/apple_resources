

- AVFoundation
- AVCaption
-  AVCaption.TextAlignment 

Enumeration

# AVCaption.TextAlignment

Text alignment options for a caption.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum TextAlignment
```

## Topics

### Text Alignments

case start

An alignment of the text to the start of the inline progression direction.

case end

An alignment of the text to the end of the inline progression direction.

case center

An alignment of the text to the center of the display.

case left

An alignment of the text to the left in horizontal writing mode, and top in vertical writing mode.

case right

An alignment of the text to the right in horizontal writing mode, and bottom in vertical writing mode.

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

### Accessing Alignment

var textAlignment: AVCaption.TextAlignment

The alignment for the caption text.

