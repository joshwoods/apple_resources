

- AVFoundation
-  AVCaptionRubyAlignment 

Enumeration

# AVCaptionRubyAlignment

Constants that indicate ruby text alignments.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum AVCaptionRubyAlignment
```

## Topics

### Text Alignments

case start

An alignment with the ruby base and text at the left edge of horizontal text in a left-to-right inline progression, or at top of the vertical text in a top-to-bottom inline progression.

case center

An alignment with the ruby text at the center of ruby base.

case distributeSpaceBetween

An alignment with the ruby text so the spaces between the ruby text characters are equal.

case distributeSpaceAround

An alignment with the ruby text so the spaces around each ruby text character are equal.

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

### Accessing Text Properties

var text: String

The ruby text.

var position: AVCaptionRubyPosition

The ruby text position.

enum AVCaptionRubyPosition

Constants that indicate ruby text positions.

var alignment: AVCaptionRubyAlignment

The ruby text alignment.

