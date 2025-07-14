

- AVFoundation
- AVCaption
-  AVCaption.Ruby 

Class

# AVCaption.Ruby

An object that presents ruby characters.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class Ruby
```

## Overview

Ruby characters are small annotations, typically used in Japanese content, that render alongside the base text.

## Topics

### Creating Ruby Text

init(text: String)

Creates ruby text.

convenience init(text: String, position: AVCaptionRubyPosition, alignment: AVCaptionRubyAlignment)

Creates ruby text with position and alignment.

### Accessing Text Properties

var text: String

The ruby text.

var position: AVCaptionRubyPosition

The ruby text position.

enum AVCaptionRubyPosition

Constants that indicate ruby text positions.

var alignment: AVCaptionRubyAlignment

The ruby text alignment.

enum AVCaptionRubyAlignment

Constants that indicate ruby text alignments.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Accessing Advanced Typography

func ruby(at: String.Index) -> (AVCaption.Ruby?, Range&lt;String.Index>)

Returns the ruby text at the index position.

func textCombine(at: String.Index) -> (AVCaption.TextCombine, Range&lt;String.Index>)

Returns the text combine at the index position.

enum TextCombine

The caption’s supported rendering policy options.

