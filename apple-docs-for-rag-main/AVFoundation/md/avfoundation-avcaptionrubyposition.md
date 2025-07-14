

- AVFoundation
-  AVCaptionRubyPosition 

Enumeration

# AVCaptionRubyPosition

Constants that indicate ruby text positions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum AVCaptionRubyPosition
```

## Topics

### Ruby Positions

case before

Display ruby text above horizontal text, or to the right of vertical text in a right-to-left block progression.

case after

Display ruby text below horizontal text, or to the left of vertical text in a right-to-left block progression.

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

var alignment: AVCaptionRubyAlignment

The ruby text alignment.

enum AVCaptionRubyAlignment

Constants that indicate ruby text alignments.

